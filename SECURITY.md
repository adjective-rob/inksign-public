# Security Policy

Inksign signs documents and handles cryptographic keys, so we take security seriously and
welcome reports from the community.

## Reporting a vulnerability

**Please report security issues privately — do not open a public issue.**

Use GitHub's **[private vulnerability reporting](https://github.com/adjective-rob/inksign-public/security/advisories/new)**
(on this repo: **Security → Advisories → _Report a vulnerability_**). It opens a private,
encrypted channel between you and the maintainers — built for exactly this.

Please include enough to reproduce: affected version and platform, steps, and the impact
you observed.

### What to expect

- **Acknowledgement within 3 business days.**
- An assessment and, where valid, a fix timeline — we'll keep you updated.
- Credit in the release notes if you'd like it (or stay anonymous).

Please give us a reasonable window to release a fix before any public disclosure. We do
not currently run a paid bug-bounty program, but we're grateful for responsible reports.

## Scope

In scope:

- The **Inksign desktop application** (signing core, CLI, MCP server, Electron GUI).
- The **inksign.org** website and its in-browser signature verifier.

Examples of what we especially care about: anything that could expose or exfiltrate a
private key, forge or silently alter a signature, cause the verifier to accept an invalid
or tampered document, or bypass the authorize→sign separation.

Out of scope: findings that require a already-compromised machine or physical access,
social-engineering, and reports about third-party services (e.g. your OS keyring, GitHub,
or the hosting provider) that we don't control.

## Supported versions

Inksign is pre-1.0. Security fixes target the **latest release**; please reproduce against
it before reporting.

## Our security posture

Inksign is designed to minimize what can go wrong:

- **Keys never leave your machine.** Signing happens locally; no key material is ever
  transmitted, and it can live in software, a TPM, or a hardware token.
- **No telemetry, no uploads.** The app sends nothing home; the web verifier runs entirely
  in your browser.
- **Standards-based.** Signatures are PAdES (ETSI / ISO), verifiable by any compliant tool.
- **Authorize and sign are separate steps** internally, so signing always acts on a
  digest bound at authorization time rather than silently re-reading a changed file.

Thank you for helping keep Inksign and its users safe.
