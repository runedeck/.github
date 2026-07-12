# Security

## Reporting a Vulnerability

Email **martin.zeman@pm.me** with `[runedeck security]` in the subject. Include the affected repo and file, reproduction steps, and impact. Expect acknowledgement within 72 hours.

## Supply Chain

Rune Deck repositories pin third-party GitHub Actions to immutable refs, verify remotely fetched scripts by SHA-256 before execution, and record provenance (in-toto/SLSA sidecars) for content adopted from external sources. Reports about gaps in any of these are in scope.
