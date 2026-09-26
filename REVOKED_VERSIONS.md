# Revoked versions

- `0.3.0.0`: revoked before distribution because the published `.appinstaller` text normalization did not match its recorded SHA-256. The signed MSIX and certificate hashes matched, but this release must not be installed.
- `0.3.0.1`: revoked before distribution because its `.appinstaller` root schema required Windows 11 even though the application supports Windows 10. The signed MSIX itself was not affected; use `0.3.0.2` or newer.