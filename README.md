<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/inksign-logo-dark.svg">
  <img src="./assets/inksign-logo-light.svg" alt="Inksign" width="300">
</picture>

### Sign PDFs on your own machine. Your keys never leave it.

[![Latest release](https://img.shields.io/github/v/release/adjective-rob/inksign-public?label=latest&color=2c46d8)](https://github.com/adjective-rob/inksign-public/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/adjective-rob/inksign-public/total?color=2c46d8)](https://github.com/adjective-rob/inksign-public/releases)
![Platform: Linux](https://img.shields.io/badge/platform-Linux-333)

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

| Your system | File | Install |
|---|---|---|
| **Debian / Ubuntu** | `Inksign-amd64.deb` | Double-click, or `sudo dpkg -i Inksign-amd64.deb` |
| **Fedora / RHEL / openSUSE** | `Inksign-x86_64.rpm` | Double-click, or `sudo dnf install ./Inksign-x86_64.rpm` |
| _Any distro (AppImage)_ | — | _Coming soon_ |

Then search **"Inksign"** in your app menu and open it. Your existing keys are picked up
automatically — open a PDF, place your signature, and seal it.

## Verify a signature

Received a signed PDF? Check it **in your browser** — nothing is uploaded — at
[**inksign.org/v**](https://inksign.org/v): it confirms the signature is cryptographically
intact, covers the whole document, and matches the signer.

## Prepare, then sign

Build the document you need to sign without leaving Inksign — everything stays on your
machine:

- **Combine PDFs** into one file, in order.
- **Split a PDF** — pull out specific pages, or burst every page into its own file.
- **Markdown & Word (`.docx`) → PDF**, ready to sign.

Each produces an ordinary, unsigned PDF you then seal with a signature.

## Why Inksign

- **Your keys never leave the machine.** Signing happens locally; no telemetry, no upload.
- **Standards-based.** PAdES signatures (ETSI / ISO), verifiable in Acrobat and any
  compliant reader — not a proprietary format.
- **Honest.** Ink marks say they stay editable; cryptographic seals say they don't.
  Inksign never claims a legal tier it can't back.

## Issues & security

- Bugs and feature requests: the [issue tracker](https://github.com/adjective-rob/inksign-public/issues).
- Found a vulnerability? Please report it privately — see [SECURITY.md](./SECURITY.md).

## License

Inksign is proprietary software. Copyright © Adjective LLC. All rights reserved. The
downloadable builds are licensed for use under their accompanying terms; this repository
hosts those downloads and issue tracking only. See [inksign.org/terms](https://inksign.org/terms).
