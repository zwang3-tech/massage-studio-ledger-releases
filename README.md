# Massage Studio Ledger — signed internal releases

This public repository contains only signed MSIX packages, the public trust certificate, checksums, and update metadata. It contains no source code, OAuth credentials, ledger data, or private signing keys.

Current version: 0.11.0.2

## Install on another Windows PC

**Direct installer:** [Open MassageStudioLedger.appinstaller](https://zwang3-tech.github.io/massage-studio-ledger-releases/MassageStudioLedger.appinstaller)

On a new PC, first verify `SereneMassageInternalSigning.cer` against the SHA-256 in `SHA256SUMS.txt`, then import it to **Local Computer → Trusted People** with administrator approval. This one-time trust step is required for this privately signed app. Never put the certificate in Trusted Root Certification Authorities. After that, open the direct installer link above and confirm the publisher is **Serene Massage LLC**.

To have an assistant guide the installation, provide this repository URL and say: “Please follow the README to install Massage Studio Ledger on this Windows PC. Verify the signing certificate first; stop and ask me before administrator approval, Google sign-in, or any Windows security prompt. Do not disable Defender or SmartScreen, and do not run unreviewed scripts.”

After installation, connect Google Sheets from the app on this PC. Google authorization is per device; do not share passwords, OAuth secrets, or tokens in chat or this repository.

Versions `0.3.0.0` and `0.3.0.1` are revoked. Use `0.3.0.2` or newer.