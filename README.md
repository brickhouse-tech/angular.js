AngularJS LTS — Community Security Patches
===========================================

> **This is a community-maintained fork of AngularJS 1.x** providing security patches for known CVEs.
> The original AngularJS project reached End-of-Life in January 2022 and no longer receives updates.

## Why This Fork?

AngularJS still has **~2 million monthly npm downloads**. Thousands of enterprise applications depend on it.
The only alternative for security patches was expensive commercial support ($15K–$50K+/year).
This fork provides **free, open-source security patches** as a drop-in replacement.

## What's Included

- ✅ **8 CVE/vulnerability fixes** (2 HIGH, 6 MEDIUM) — see table below
- ✅ **Drop-in replacement** — same API, same behavior, just patched
- ✅ **CI via GitHub Actions** — tested on Node 20
- ✅ **OIDC npm publishing** with provenance
- ✅ **MIT licensed** — same as upstream

## Security Patches

| CVE / Snyk ID | Severity | Type | Status |
|---|---|---|---|
| SNYK-JS-ANGULAR-6091113 | **HIGH** | ReDoS in `ng-srcset` directive | ✅ Fixed |
| CVE-2022-25844 | **HIGH** | ReDoS in `angular.copy` | ✅ Fixed |
| SNYK-JS-ANGULAR-9919773 | Medium | SVG `<image>` href sanitization bypass | ✅ Fixed |
| SNYK-JS-ANGULAR-7924843 | Medium | `srcset` allowlist bypass | ✅ Fixed |
| SNYK-JS-ANGULAR-7924842 | Medium | `<source>` srcset not sanitized | ✅ Fixed |
| SNYK-JS-ANGULAR-3373046 / CVE-2020-7212 | Medium | ReDoS in URL input validation | ✅ Fixed |
| SNYK-JS-ANGULAR-3373045 | Medium | ReDoS in `$resource` service | ✅ Fixed |
| CVE-2020-7676 | Medium | Prototype pollution via `merge`/`copy` | ✅ Fixed |
| SNYK-JS-ANGULAR-2949781 | Medium | XSS via `<textarea>` (IE-specific) | 🔄 Planned |
| SNYK-JS-ANGULAR-2772735 | Medium | ReDoS in locale number formatting | 🔄 Planned |
| CVE-2022-25869 | Medium | `$sanitize` bypass via `<style>` (IE/Edge) | 🔄 Planned |

## Installation

```bash
npm install @brickhouse-tech/angular-lts
```

Drop-in replacement for `angular@1.8.3`. Same API, same behavior.

## Migration from `angular`

```diff
- "angular": "1.8.3"
+ "@brickhouse-tech/angular-lts": "^1.8.4"
```

No code changes required.

## Sponsorship

This project is maintained by [Brickhouse Tech](https://github.com/brickhouse-tech).
If your organization depends on AngularJS, consider sponsoring to ensure continued maintenance.

[![Sponsor](https://img.shields.io/badge/sponsor-brickhouse--tech-blue?logo=github)](https://github.com/sponsors/brickhouse-tech)

| Tier | Price | Benefits |
|------|-------|----------|
| Community | Free | Open source patches, npm package |
| Supporter | $50/mo | Logo on README, priority issues |
| Professional | $500/mo | 48h SLA, private Slack, migration guidance |
| Enterprise | $5,000/mo | 4h SLA, custom patches, compliance docs |

## Versioning

This fork follows the upstream `1.8.x` line. Security patches are published as `1.8.4+` releases.
Prerelease versions use the format `1.8.4-N`.

## License

MIT — same as the original AngularJS project. See [LICENSE](LICENSE).

## Links

- **npm**: [@brickhouse-tech/angular-lts](https://www.npmjs.com/package/@brickhouse-tech/angular-lts)
- **Original project**: [angular/angular.js](https://github.com/angular/angular.js) (archived)
- **HeroDevs NES** (commercial alternative): [herodevs.com](https://www.herodevs.com/support/angularjs-nes)
