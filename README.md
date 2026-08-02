<div align="center">

# Inksign

**Sign PDFs on your own machine. Your keys never leave it.**

[Website](https://inksign.org) · [Verify a signed PDF](https://inksign.org/v) · [Download](#download) · [Report an issue](https://github.com/adjective-rob/inksign-public/issues)

</div>

Inksign seals documents with standards-based **PAdES** signatures, entirely on your
computer. No cloud, no account, no upload — your private key can live in a software
keystore, your **TPM**, or a hardware token, and it never leaves the machine.

This repository is the **public home for Inksign downloads and issue tracking**. The
application source is not published here.

## Download

Inksign runs on Linux. Grab the format for your system from the
[**latest release**](https://github.com/adjective-rob/inksign-public/releases/latest):

| Your system | File | How to install |
|---|---|---|
| **Debian / Ubuntu** | `.deb` | Double-click to install — Inksign appears in your app menu. |
| **Fedora / openSUSE** | `.rpm` | Double-click to install — with the menu entry. |
| **Any distro** | `AppImage` | `chmod +x Inksign-*.AppImage` and run it. No install. |

> First release coming soon.

## Verify a signature

Received a signed PDF? You can check it **in your browser** — nothing is uploaded —
at [**inksign.org/v**](https://inksign.org/v): it confirms the signature is
cryptographically intact, covers the whole document, and matches the signer.

## Why Inksign

- **Your keys never leave the machine.** Signing happens locally; no telemetry, no upload.
- **Standards-based.** PAdES signatures (ISO / eIDAS), verifiable in Acrobat and any
  compliant reader — not a proprietary format.
- **Honest.** Ink marks say they stay editable; cryptographic seals say they don't.
  Inksign never claims a legal tier it can't back.

## Issues & feedback

Bug reports and feature requests are welcome in the
[issue tracker](https://github.com/adjective-rob/inksign-public/issues).

## License

Inksign is proprietary software. Copyright © Adjective LLC. All rights reserved.
The downloadable builds are licensed for use under their accompanying terms; this
repository hosts those downloads and issue tracking only.
