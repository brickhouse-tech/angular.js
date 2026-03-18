# AngularJS 1.x Security Patches — Free, Drop-in, MIT Licensed

[![npm version](https://img.shields.io/npm/v/@brickhouse-tech/angular-lts?logo=npm)](https://www.npmjs.com/package/@brickhouse-tech/angular-lts)
[![npm downloads](https://img.shields.io/npm/dm/@brickhouse-tech/angular-lts)](https://www.npmjs.com/package/@brickhouse-tech/angular-lts)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![CVEs Patched](https://img.shields.io/badge/CVEs%20Patched-11-green)](https://github.com/brickhouse-tech/angular.js/blob/master/SECURITY.md)

> **Production-ready security patches for AngularJS 1.x** — All 11 known CVEs patched. Zero code changes required. Open source alternative to $15K–$50K/year commercial support.

**[Try the Live Demo →](https://brickhouse-tech.github.io/angular-lts-demo/)**

---

## The Problem

AngularJS reached **End-of-Life in January 2022**. Google stopped all maintenance and security updates.

Yet the framework still has:
- **~2 million monthly downloads** on npm
- Thousands of production applications in Fortune 500 companies
- **11 unpatched security vulnerabilities** (2 HIGH, 9 MEDIUM severity)
- No official migration path that doesn't require a complete rewrite

Most enterprises face three bad options:
1. **Stay on 1.8.3** with known CVEs → fails security audits, compliance reviews
2. **Rewrite to modern Angular/React/Vue** → $500K+ and 12–24 months
3. **Pay $15K–$50K+/year** for commercial Extended Support

---

## The Solution

**@brickhouse-tech/angular-lts** is a community-maintained fork that patches all known security vulnerabilities in AngularJS 1.x.

✅ **All 11 CVEs patched** — 2 HIGH, 9 MEDIUM severity vulnerabilities fixed  
✅ **Drop-in replacement** — Same API, same behavior, zero code changes  
✅ **MIT licensed** — Free and open source, forever  
✅ **Actively maintained** — CI/CD, npm provenance, GitHub security advisories  
✅ **Production-ready** — Latest version **1.9.3** on npm

**One command. Zero refactoring. Full security compliance.**

---

## Security Vulnerabilities Patched

| # | Vulnerability ID | Severity | CVSS | Vulnerability Type | Status |
|---|-----------------|----------|------|-------------------|--------|
| 1 | [SNYK-JS-ANGULAR-9919773](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-9919773) | Medium | 5.3 | Incomplete Filtering (SVG href) | ✅ Fixed in 1.8.4+ |
| 2 | [SNYK-JS-ANGULAR-7924843](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-7924843) | Medium | 5.3 | srcset bypass | ✅ Fixed in 1.8.4+ |
| 3 | [SNYK-JS-ANGULAR-7924842](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-7924842) | Medium | 5.3 | srcset source spoofing | ✅ Fixed in 1.8.4+ |
| 4 | [SNYK-JS-ANGULAR-6091113](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-6091113) | **High** | 7.5 | ReDoS ng-srcset | ✅ Fixed in 1.8.4+ |
| 5 | [SNYK-JS-ANGULAR-3373044](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-3373044) | Medium | 5.3 | ReDoS angular.copy() | ✅ Fixed in 1.8.4+ |
| 6 | [SNYK-JS-ANGULAR-3373046](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-3373046) | Medium | 5.3 | ReDoS input[type=url] | ✅ Fixed in 1.8.4+ |
| 7 | [SNYK-JS-ANGULAR-3373045](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-3373045) | Medium | 5.3 | ReDoS $resource | ✅ Fixed in 1.8.4+ |
| 8 | [SNYK-JS-ANGULAR-2949781](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-2949781) | Medium | 6.1 | XSS textarea (IE) | ✅ Fixed in 1.8.4+ |
| 9 | [SNYK-JS-ANGULAR-2772735](https://security.snyk.io/vuln/SNYK-JS-ANGULAR-2772735) | Medium | 5.3 | ReDoS DATE_FORMATS | ✅ Fixed in 1.8.4+ |
| 10 | [CVE-2022-25869](https://nvd.nist.gov/vuln/detail/CVE-2022-25869) | Medium | 6.1 | $sanitize bypass style (IE/Edge) | ✅ Fixed in 1.8.4+ |
| 11 | [CVE-2022-25844](https://nvd.nist.gov/vuln/detail/CVE-2022-25844) / [CVE-2020-7676](https://nvd.nist.gov/vuln/detail/CVE-2020-7676) / [CVE-2020-7212](https://nvd.nist.gov/vuln/detail/CVE-2020-7212) | High+Medium | 7.5 | ReDoS + XSS + Proto Pollution | ✅ Fixed in 1.8.4+ |

**All patches tested and verified.** Full details in [SECURITY.md](SECURITY.md).

---

## Migration Guide

### Step 1: Uninstall the old package
```bash
npm uninstall angular
```

### Step 2: Install @brickhouse-tech/angular-lts
```bash
npm install @brickhouse-tech/angular-lts
```

**That's it.** No code changes. No configuration. No build changes. Same API, same behavior, just patched.

Your `package.json` should now show:
```json
{
  "dependencies": {
    "@brickhouse-tech/angular-lts": "^1.9.3"
  }
}
```

If you're using a CDN, point to:
```html
<script src="https://unpkg.com/@brickhouse-tech/angular-lts@1.9.3/angular.min.js"></script>
```

---

## @brickhouse-tech/angular-lts vs. HeroDevs NES

HeroDevs offers commercial Extended Support for AngularJS (NES). It's a solid option for enterprises that need vendor backing. But it's expensive — and unnecessary for most teams.

| Feature | @brickhouse-tech/angular-lts | HeroDevs NES |
|---------|------------------------------|--------------|
| **Price** | **Free (MIT)** | **$15,000–$50,000+/year** |
| **Security patches** | ✅ All 11 CVEs patched | ✅ All known CVEs patched |
| **Drop-in replacement** | ✅ Zero code changes | ✅ Zero code changes |
| **Open source** | ✅ MIT license, public repo | ❌ Proprietary, closed source |
| **npm package** | ✅ Public npm | ✅ Private npm registry |
| **Community support** | ✅ GitHub issues | ❌ Paid support only |
| **SLA** | ❌ Best-effort (Enterprise tier available) | ✅ Contractual SLA |
| **Custom patches** | ❌ (Enterprise tier available) | ✅ Custom backports |
| **Compliance docs** | ❌ (Enterprise tier available) | ✅ Audit reports, attestations |

**Bottom line:** If you just need the CVEs patched, use @brickhouse-tech/angular-lts and save $15K–$50K/year. If you need vendor SLAs and compliance paperwork, consider our Enterprise tier or HeroDevs.

---

## Enterprise Support

Need more than open source patches? We offer commercial support tiers for teams that require SLAs, priority patches, or custom backports.

| Tier | Price | What You Get |
|------|-------|--------------|
| **Community** | **Free** | Open source patches, GitHub issues, npm package |
| **Professional** | **$500/month** | 48-hour SLA, private Slack channel, priority bug fixes |
| **Enterprise** | **$5,000/month** | 4-hour SLA, custom patches, compliance documentation, audit support |

**[Get Enterprise Support →](https://brickhouse-tech.lemonsqueezy.com)**

---

## Support This Project

This fork is maintained by [Brickhouse Tech](https://github.com/brickhouse-tech) and community contributors. If your organization depends on AngularJS, consider sponsoring to ensure continued maintenance and faster patch releases.

**[Sponsor on GitHub →](https://github.com/sponsors/brickhouse-tech)**

Every contribution helps keep this project alive for the thousands of teams still running AngularJS in production.

---

## Technical Details

- **Upstream:** Based on `angular@1.8.3` (final official release)
- **Current version:** `1.9.3` (includes all security patches)
- **Testing:** CI via GitHub Actions, tested on Node 20+
- **Publishing:** OIDC npm publishing with provenance attestation
- **License:** MIT (same as original AngularJS)

---

## Links

- **npm:** [@brickhouse-tech/angular-lts](https://www.npmjs.com/package/@brickhouse-tech/angular-lts)
- **Demo:** [https://brickhouse-tech.github.io/angular-lts-demo/](https://brickhouse-tech.github.io/angular-lts-demo/)
- **Security advisories:** [SECURITY.md](SECURITY.md)
- **Original project:** [angular/angular.js](https://github.com/angular/angular.js) (archived)
- **GitHub Sponsors:** [https://github.com/sponsors/brickhouse-tech](https://github.com/sponsors/brickhouse-tech)
- **Enterprise Support:** [https://brickhouse-tech.lemonsqueezy.com](https://brickhouse-tech.lemonsqueezy.com)

---

## License

MIT — same as the original AngularJS project. See [LICENSE](LICENSE) for full text.

---

**Built with ❤️ by [Brickhouse Tech](https://github.com/brickhouse-tech) and community contributors.**
