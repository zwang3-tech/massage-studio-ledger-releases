# Massage Studio Ledger — signed internal releases

This public repository contains only signed MSIX packages, the public trust certificate, checksums, and update metadata. It contains no source code, OAuth credentials, ledger data, or private signing keys.

Current version: 0.3.0.1

Install the public certificate into **Current User → Trusted People**, then download and open `MassageStudioLedger.appinstaller`.

Version `0.3.0.0` is revoked because Git line-ending normalization changed the published `.appinstaller` hash. The signed MSIX itself was not affected; use `0.3.0.1` or newer.