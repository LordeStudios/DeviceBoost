# Security Policy

## Supported versions

| Version | Supported |
|---|---|
| 0.1.x | Yes |

## Reporting a vulnerability

Please report vulnerabilities through [GitHub's private vulnerability reporting](https://github.com/LordeStudios/DeviceBoost/security/advisories/new). Do not open public issues for security problems.

When reporting, include:

- The DeviceBoost version and the Windows version affected.
- A description of the issue and how it could be reproduced.
- Any relevant logs, without credentials or tokens.

## Scope notes

- The host service binds to loopback only (`127.0.0.1`) and requires an admin token header for its API. Reports about exposing these ports externally are out of scope by design.
- Pairing tokens are single use and time limited (600 seconds maximum) by design.
