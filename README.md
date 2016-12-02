# openssl-bin
Binary builds of several OpenSSL versions for the purpose of CI. Nothing to see here really.

Build command:
```
./config --prefix=/opt/openssl-1.X.Yz --openssldir=/opt/openssl-1.X.Yz shared no-engines no-hw
make && make install
```

- Yeah, that requires root privileges on normal machines, but I'm doing it in a VM. Call the cops, I don't care.
- 1.1.x branch doesn't need `no-engines`
- Man pages not included