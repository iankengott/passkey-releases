# Passkey releases

Signed release files for the Passkey demo key: the PC installer and key firmware. The installer on the key's setup drive checks this repository's latest release for a newer version.

Every release carries `index.json` and `index.json.sig`. The signature is Ed25519 over `PKU-INDEX-V1\0` followed by the exact bytes of `index.json`, made with the project release key. The installer and the key firmware carry the public key and refuse anything it did not sign. Firmware files (`.pkur`) are signed the same way.

Release public key (`RELEASE-PUBLIC-KEY.hex`), key id `55265bdb0f5f7e17`:

```
8aba6fcdf41618fe46c8e4ca1ca8ebd0f6a84e303a117de2f00a109a0e46e24e
```

This is demo software. The Windows programs are not code-signed, so Windows shows a SmartScreen warning the first time. No device is sold here.
