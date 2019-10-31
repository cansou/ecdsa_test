# ecdsa_test
C++ test program using OpenSSL library for NID_X9_62_prime256v1 Elliptic Curve signature verification

# Build
To build on macOS
```
g++ -g -lssl -std=c++11  main.cpp -o testECDSA -lcrypto -I/usr/local/Cellar/openssl/1.0.2p/include/
```

To build on RPi or Linux
```
g++ -g -lssl -std=c++11  main.cpp -o testECDSA -lcrypto
```

# Test

```
./testECDSA
ECDSA Test Engine  
>>> BUFFER = 4C42D6050000009AFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF000102030405060708090A0B0C0D0E0F101112131415161718191A1B1C1D1E1F000000
>>> SHA256 = 6EB92E2F6F64FAD56BA5195B34921D6F93F236D4086DC6B98EBF61AFDF7CC075
Verifed EC Signature

Process finished with exit code 0
```
