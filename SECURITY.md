# Security

## Reporting a Vulnerability

Email **martin.zeman@pm.me** with `[runedeck security]` in the subject. Include the affected repo and file, reproduction steps, and impact. Expect acknowledgement within 72 hours.

## Release Signing

Releases are vouched for by owner-signed annotated tags. The signing key:

```text
786F851F8AE345F5A98B822EC92F47D08BCD9F72
```

The armored public key is published at [keys.openpgp.org](https://keys.openpgp.org) and ships as the root `KEYS` file in the [skeleton](https://github.com/runedeck/skeleton) baseline that scaffolds each repository. Verify a release with `git verify-tag vX.Y.Z` against a keyring holding that fingerprint. This page is the out-of-band anchor: if a `KEYS` file ever disagrees with the fingerprint above, trust this page and report it.

## Supply Chain

Rune Deck repositories pin third-party GitHub Actions to immutable refs, verify remotely fetched scripts by SHA-256 before execution, and record provenance (in-toto/SLSA sidecars) for content adopted from external sources. Reports about gaps in any of these are in scope.
