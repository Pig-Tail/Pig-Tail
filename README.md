<h1 align="center">Jorge González Milla</h1>
<p align="center"><b><code>Pig-Tail</code></b> · Offensive Security Engineer · Vulnerability Researcher · Red Teamer</p>
<p align="center">
  <img src="https://img.shields.io/badge/Assigned_CVEs-23-b5185c?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Published_advisories-31-e5654a?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Vulns_reported-176+-d9822b?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Projects-60+-56b6c2?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Since-2017-8b95a5?labelColor=24292f&style=flat-square">
  <a href="https://twitter.com/jgonzalezmilla"><img src="https://img.shields.io/badge/X-@jgonzalezmilla-1DA1F2?logo=x&logoColor=white&style=flat-square"></a>
</p>

---

### `whoami`

Offensive security engineer and vulnerability researcher. I audit widely-used open-source and
commercial software for **credible, exploitation-defensible bugs** and drive them through
coordinated disclosure — attack-surface mapping → taint tracking → a **working PoC** → a
defensible CVSS write-up. Comfortable across web/API stacks, C/C++ memory safety,
Go/Rust/PHP/Python, and red-team tooling.

- 🔭 **Classes I hunt:** RCE &amp; command/arg injection · auth/authz bypass, IDOR &amp; tenant escape · SSRF · path traversal / zip-slip · unsafe deserialization · memory corruption · race/TOCTOU.
- 🧪 **How I verify:** local instance + benign PoC (sentinel / timing oracle), then an adversarial re-read to kill false positives. No theoretical reports.
- 🛡️ **Background:** red-team infrastructure &amp; malware-dev tradecraft (see certifications).

---

### 🎯 Assigned CVEs (23)

| CVE | Project | Vulnerability | GitHub |
|:--|:--|:--|:--|
| [**CVE-2026-14620**](https://www.cve.org/CVERecord?id=CVE-2026-14620) | `webpack-dev-server` | webpack-dev-server vulnerable to cross-site request forgery via internal | [advisory](https://github.com/webpack/webpack-dev-server/security/advisories/GHSA-f5vj-f2hx-8m93) |
| [**CVE-2026-40936**](https://www.cve.org/CVERecord?id=CVE-2026-40936) | `glpi-agent` | ToolBox plugin can allow unauthenticated path traversal leading to arbit | — |
| [**CVE-2026-42187**](https://www.cve.org/CVERecord?id=CVE-2026-42187) | `glpi-agent` | Proxy plugin can allow arbitrary file write if `local_store` is enabled | — |
| [**CVE-2026-45621**](https://www.cve.org/CVERecord?id=CVE-2026-45621) | `glpi-agent` | MongoDB inventory module allows JavaScript injection via unescaped login | — |
| [**CVE-2026-46615**](https://www.cve.org/CVERecord?id=CVE-2026-46615) | `glpi-agent` | Database inventory modules execute OS commands with unsanitized database | — |
| [**CVE-2026-48728**](https://www.cve.org/CVERecord?id=CVE-2026-48728) | `glpi-inventory-plugin` | Job enumeration and status manipulation on Deploy, Collect, and ESX agen | [advisory](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-xj72-9f7x-f4hm) |
| [**CVE-2026-48730**](https://www.cve.org/CVERecord?id=CVE-2026-48730) | `glpi-inventory-plugin` | Reflected XSS | — |
| [**CVE-2026-49285**](https://www.cve.org/CVERecord?id=CVE-2026-49285) | `glpi-agent` | OS Command Injection in GLPI Agent ToolBox Results export via unsanitize | — |
| [**CVE-2026-52764**](https://www.cve.org/CVERecord?id=CVE-2026-52764) | `glpi-agent` | MSSQL inventory module executes OS commands with unsanitized database na | — |
| [**CVE-2026-52765**](https://www.cve.org/CVERecord?id=CVE-2026-52765) | `glpi-agent` | Oracle and DB2 inventory modules allow SQL injection in GLPI server-supp | — |
| [**CVE-2026-52768**](https://www.cve.org/CVERecord?id=CVE-2026-52768) | `glpi-agent` | Deploy task Path Traversal in Tools::Archive | — |
| [**CVE-2026-53626**](https://www.cve.org/CVERecord?id=CVE-2026-53626) | `glpi` | Arbitrary document read | — |
| [**CVE-2026-54697**](https://www.cve.org/CVERecord?id=CVE-2026-54697) | `cbssh` | Excessive allocation and integer overflow in DER private-key parsing | [advisory](https://github.com/connectbot/cbssh/security/advisories/GHSA-vc8p-8pxg-rfwg) |
| [**CVE-2026-54764**](https://www.cve.org/CVERecord?id=CVE-2026-54764) | `traefik` | ForwardAuth middleware leaks X-Forwarded-Port spoofing via untrusted X-F | [advisory](https://github.com/traefik/traefik/security/advisories/GHSA-3q9r-p662-5j8m) |
| [**CVE-2026-55422**](https://www.cve.org/CVERecord?id=CVE-2026-55422) | `conda-forge` | Stored DOM XSS on conda-forge.org via unsanitized dangerouslySetInnerHTM | [advisory](https://github.com/conda-forge/conda-forge.github.io/security/advisories/GHSA-r5vj-wgjv-r524) |
| [**CVE-2026-55780**](https://www.cve.org/CVERecord?id=CVE-2026-55780) | `NanaZip` | Uncaught exception / unbounded allocation in NanaZip .NET single-file Ex | [advisory](https://github.com/M2Team/NanaZip/security/advisories/GHSA-ppm9-5267-rq72) |
| [**CVE-2026-55781**](https://www.cve.org/CVERecord?id=CVE-2026-55781) | `NanaZip` | Unbounded memory allocation (DoS) in NanaZip UFS parser via unvalidated  | [advisory](https://github.com/M2Team/NanaZip/security/advisories/GHSA-m34h-jf84-m74h) |
| [**CVE-2026-55782**](https://www.cve.org/CVERecord?id=CVE-2026-55782) | `NanaZip` | Unbounded memory allocation (DoS) in NanaZip WebAssembly parser via atta | [advisory](https://github.com/M2Team/NanaZip/security/advisories/GHSA-qxhc-2v6p-wm8m) |
| [**CVE-2026-55783**](https://www.cve.org/CVERecord?id=CVE-2026-55783) | `NanaZip` | NULL pointer dereference in Extract() of all seven NanaZip custom archiv | [advisory](https://github.com/M2Team/NanaZip/security/advisories/GHSA-q67r-9cfh-xc29) |
| [**CVE-2026-57562**](https://www.cve.org/CVERecord?id=CVE-2026-57562) | `readest` | Subscription/entitlement hijack: /api/stripe/check binds any paid Checko | — |
| [**CVE-2026-57565**](https://www.cve.org/CVERecord?id=CVE-2026-57565) | `readest` | Cross-tenant object write via unsanitized fileName in /api/storage/uploa | — |
| [**CVE-2026-57566**](https://www.cve.org/CVERecord?id=CVE-2026-57566) | `readest` | Unauthenticated SSRF / open request proxy in /api/opds/proxy | — |
| [**CVE-2026-57567**](https://www.cve.org/CVERecord?id=CVE-2026-57567) | `readest` | Unscoped Tauri IPC download_file/upload_file allow arbitrary local file  | — |

<sub>CVE records are public at cve.org; some GitHub advisories are resolved privately (no public advisory page).</sub>

---

### 🐛 Published GitHub advisories (no CVE assigned) (22)

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `nebula-mesh` | Certificate revocation is never enforced at the mesh: nebula-agent drops the pol | CWE-299/CWE-672 | [`GHSA-cm26-5974-52h8`](https://github.com/forgekeep/nebula-mesh/security/advisories/GHSA-cm26-5974-52h8) |
| `nodemailer` | Message-level raw option bypasses disableFileAccess/disableUrlAccess, enabling a | CWE-73/CWE-918 | [`GHSA-p6gq-j5cr-w38f`](https://github.com/nodemailer/nodemailer/security/advisories/GHSA-p6gq-j5cr-w38f) |
| `shopper` | Missing authorization on product variant DeleteAction/DeleteBulkAction in Form\V | CWE-285/CWE-862 | [`GHSA-93v2-gcw2-vfwc`](https://github.com/shopperlabs/shopper/security/advisories/GHSA-93v2-gcw2-vfwc) |
| `horilla-hr` | Server-Side Template Injection (SSTI) in Mail Preview Endpoints Allows Authentic | CWE-94/CWE-200 | [`GHSA-9p83-4w63-7c24`](https://github.com/horilla/horilla-hr/security/advisories/GHSA-9p83-4w63-7c24) |
| `monitoring-plugins` | fetch() forwards credential headers across a cross-origin redirect | CWE-200/CWE-918 | [`GHSA-4jc5-g844-4x33`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-4jc5-g844-4x33) |
| `monitoring-plugins` | SSRF and auth-token disclosure via unvalidated @odata.id link in redfish-* plugi | CWE-20/CWE-200/CWE-918 | [`GHSA-96fx-pqc3-28xv`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-96fx-pqc3-28xv) |
| `probo` | Cross-tenant IDOR via unvalidated FK references | CWE-639 | [`GHSA-c74x-79w6-63jh`](https://github.com/getprobo/probo/security/advisories/GHSA-c74x-79w6-63jh) |
| `statamic` | Missing authorization on navigation endpoint allows disclosure of restricted ent | CWE-639/CWE-862 | [`GHSA-qh8c-7588-qfrv`](https://github.com/statamic/cms/security/advisories/GHSA-qh8c-7588-qfrv) |
| `surrealdb` | SSRF via JWKS URL — Redirect Following in JWT Key Fetch | CWE-918 | [`GHSA-h5rg-8p7f-47g2`](https://github.com/surrealdb/surrealdb/security/advisories/GHSA-h5rg-8p7f-47g2) |
| `glpi-agent` | Oracle inventory module uses unvalidated process username in shell su command | CWE-78 | [`GHSA-vwv6-85p7-mjvc`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-vwv6-85p7-mjvc) |
| `glpi-agent` | Collect task compiles server-controlled regular expression without validation | CWE-1333 | [`GHSA-mgcf-xgv7-5w4x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-mgcf-xgv7-5w4x) |
| `glpi-agent` | Stored XSS via SNMP community/authprotocol credential fields in ToolBox plugin | CWE-79 | [`GHSA-cwg9-jj5m-pq4q`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-cwg9-jj5m-pq4q) |
| `monitoring-plugins` | Symlink following in logfile legacy database migration | CWE-59/CWE-367 | [`GHSA-w2gg-hx6w-24w3`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-w2gg-hx6w-24w3) |
| `openproject` | Content Security Policy img-src wildcard enables cross-origin pixel tracking and | CWE-200 | [`GHSA-m5p8-h274-f7w8`](https://github.com/opf/openproject/security/advisories/GHSA-m5p8-h274-f7w8) |
| `formie` | Integration `form-settings` action allows SSRF and exfiltration of stored integration credentials | CWE-862/CWE-918/CWE-915 | [`GHSA-v3f3-cmj4-cvj9`](https://github.com/verbb/formie/security/advisories/GHSA-v3f3-cmj4-cvj9) |
| `formie` | Missing authorization on the sent-notification resend modal exposes submission PII | CWE-200/CWE-639/CWE-862 | [`GHSA-9rg8-2wvr-fgjh`](https://github.com/verbb/formie/security/advisories/GHSA-9rg8-2wvr-fgjh) |
| `formie` | Unauthenticated users can overwrite another user's incomplete submission via the `submit` action | CWE-639/CWE-862 | [`GHSA-584p-f93j-wpgc`](https://github.com/verbb/formie/security/advisories/GHSA-584p-f93j-wpgc) |
| `formie` | `save-submission` allows anonymous submission creation and privileged parameter override (captcha/spam bypass) | CWE-693/CWE-862/CWE-915 | [`GHSA-5mv8-8rcv-wp5f`](https://github.com/verbb/formie/security/advisories/GHSA-5mv8-8rcv-wp5f) |
| `formie` | Stored XSS in the form-import preview via unescaped title, handle, and notification name | CWE-79 | [`GHSA-xphf-8742-29m4`](https://github.com/verbb/formie/security/advisories/GHSA-xphf-8742-29m4) |
| `probo` | Public e-signature API: any trust-center visitor can complete another visitor's NDA signature and inject audit-trail events | CWE-639/CWE-862 | [`GHSA-22xj-f767-ppw6`](https://github.com/getprobo/probo/security/advisories/GHSA-22xj-f767-ppw6) |
| `probo` | Vertical privilege escalation: an org ADMIN mints an OWNER membership via `createUser`, bypassing the owner-only gate | CWE-269/CWE-863 | [`GHSA-cppp-g98f-gfpp`](https://github.com/getprobo/probo/security/advisories/GHSA-cppp-g98f-gfpp) |
| `probo` | Unauthenticated cross-tenant / hidden-item disclosure via `Query.node` in the public Trust Center API | CWE-284/CWE-639 | [`GHSA-w23w-f7v2-625w`](https://github.com/getprobo/probo/security/advisories/GHSA-w23w-f7v2-625w) |

---

### 🔬 Research &amp; vendor disclosures

- **wolfSSL — X.509 DNS name-constraint bypass** (CWE-295) · A leaf carrying a `registeredID` (or `iPAddress`) SAN sets `altNames != NULL`, which suppresses the CN-as-DNS name-constraint check in `ConfirmNameConstraints()` while the CN is still used to authenticate the peer — a **DNS-name-constrained sub-CA can impersonate arbitrary hosts**. Incomplete fix / regression of **CVE-2026-6731**. Reported with a working PoC; reproduced and fixed by wolfSSL in [PR #10837](https://github.com/wolfSSL/wolfssl/pull/10837). *(CVE pending.)*
- **wolfSSL — PKCS7 / DTLS 1.3 hardening** · Two PKCS7 non-streaming bounds over-reads (EnvelopedData IV, AuthEnvelopedData authTag) + an unbounded DTLS 1.3 `WriteDup` ACK-list growth (memory-exhaustion DoS). Fixed &amp; merged in [PR #10833](https://github.com/wolfSSL/wolfssl/pull/10833).
- **Microsoft Windows — StorSvc RPC EoP** · The Storage Service registers its ALPC/RPC interface (`44d1520b-…`) with a **NULL security callback and NULL security descriptor**, so any unprivileged local user can invoke all 36 procedures. `SvcTriggerStorageCleanup` drives `StorSvc` (SYSTEM) into `CreateProcessW("cleanmgr.exe", …)` **without impersonating the caller** → SYSTEM process creation from a standard user (missing authorization, CWE-285). Reported to MSRC — Case **111782** (VULN-180255). *(Related tooling: [alpc-toolkit](https://github.com/Pig-Tail/alpc-toolkit).)*
- **OpenStreetMap** · Reported and fixed several issues in the OSM website, **publicly credited** by the project: TOTP-cookie handling, CSP rules, and a private-message rate-limit bypass — [PR #7045](https://github.com/openstreetmap/openstreetmap-website/pull/7045) · [#7046](https://github.com/openstreetmap/openstreetmap-website/pull/7046) · [#7047](https://github.com/openstreetmap/openstreetmap-website/pull/7047) · [announcement](https://community.openstreetmap.org/t/what-s-new-on-the-openstreetmap-website/130080/30).

---

### 🔒 Under coordinated disclosure

**139+ further findings** reported across **60+ projects** are either resolved privately
(no public advisory page) or under active coordinated disclosure / vendor embargo — including
memory-safety bugs in widely-used engines, unauth secret-disclosure and RCE chains, and
supply-chain issues. Details are withheld until each vendor publishes; they surface here
automatically on disclosure.

---

### 🧰 Tools &amp; research

| Repo | What it is |
|------|------------|
| [alpc-toolkit](https://github.com/Pig-Tail/alpc-toolkit) | Rust toolkit for Windows ALPC/RPC attack-surface recon |
| [Mythic-agent-rust](https://github.com/Pig-Tail/Mythic-agent-rust) | Mythic C2 agent implemented in Rust |
| [HuntingFavicoShodan](https://github.com/Pig-Tail/HuntingFavicoShodan) | Find phishing sites by favicon hash via Shodan |
| [ReconToolTop](https://github.com/Pig-Tail/ReconToolTop) · [Recond_subdomains](https://github.com/Pig-Tail/Recond_subdomains) | Subdomain recon (alive hosts, ports, no API) |
| [Cert](https://github.com/Pig-Tail/Cert) | 📜 Certifications &amp; training (indexed) |
| [GLPI SNMP-scan PoC](https://gist.github.com/Pig-Tail/560032514a1f0506583131099ae5d686) | 📓 Gist — PoC for unauthenticated SNMP network scanning in GLPI Agent ToolBox (CWE-918) |

---

### 🎓 Certifications &amp; training (58 total)

| Category | Certifications &amp; courses (→ PDF) |
|:--|:--|
| 🔴 **Red Team / Offensive** | [MCRTA](https://github.com/Pig-Tail/Cert/blob/main/MCRTA%20Certificates.pdf) · [CRTS v2](https://github.com/Pig-Tail/Cert/blob/main/CRTS%20V2%20Certs.pdf) · [C3SA](https://github.com/Pig-Tail/Cert/blob/main/C3SA%20Premium%20Edition.pdf) · [Offensive Phishing Operations](https://github.com/Pig-Tail/Cert/blob/main/Offensive-Phishing-Operations-Certificate.pdf) · [RedInfraCraft](https://github.com/Pig-Tail/Cert/blob/main/Red%20Team%20Infrastructure%20on%20the%20Fly%20with%20RedInfraCraft.pdf) · [C2 Development](https://github.com/Pig-Tail/Cert/blob/main/C2%20Development.pdf) · [Ekoparty Red Team 101](https://github.com/Pig-Tail/Cert/blob/main/Certificado%20de%20Asistencia%20-%20Ekoparty%20Webinars%20Red%20Team%20101%20-%20jorgegonzalezmilla%40gmail.pdf) |
| 🧬 **Malware Dev / Exploitation** | [Malware Dev Essentials](https://github.com/Pig-Tail/Cert/blob/main/Malware%20Development%20Essentials-certificate.pdf) · [Malware Dev Intermediate](https://github.com/Pig-Tail/Cert/blob/main/Malware%20Development%20Intermediate-certificate.pdf) · [Adv. Process Injection v2](https://github.com/Pig-Tail/Cert/blob/main/Advance%20Process%20Injection%20V.2%20Certificate.pdf) · [OST2 Exp4011](https://github.com/Pig-Tail/Cert/blob/main/OpenSecurityTraining2%20Exp4011.pdf) · [OST2 Fuzz1001](https://github.com/Pig-Tail/Cert/blob/main/OpenSecurityTraining2%20Fuzz1001%20Certificate%20_%20OpenSecurityTraining2.pdf) · [OST2 Dbg1011](https://github.com/Pig-Tail/Cert/blob/main/OpenSecurityTraining2%20Dbg1011.pdf) · [OST2 Arch2821](https://github.com/Pig-Tail/Cert/blob/main/OpenSecurityTraining2%20Arch2821.pdf) · [OffensiveRust](https://github.com/Pig-Tail/Cert/blob/main/OffensiveRust.pdf) · [offensiveC#](https://github.com/Pig-Tail/Cert/blob/main/offensiveCsharp.pdf) · [Windows API Hooking](https://github.com/Pig-Tail/Cert/blob/main/Windows%20API%20Hooking.pdf) · [How To Write A Shellcode](https://github.com/Pig-Tail/Cert/blob/main/How%20To%20Write%20A%20Shellcode.pdf) · [Evil ClickOnce](https://github.com/Pig-Tail/Cert/blob/main/Evil%20ClickOnce%20Backdooring%20Legit%20.NET%20Application%20for%20Initial%20Access.pdf) |
| ☁️ **Cloud** | [IAM / Access Guardian](https://github.com/Pig-Tail/Cert/blob/main/Access%20Guardian_%20Mastering%20IAM%20in%20the%20Cloud.pdf) · [AWS AMI Security](https://github.com/Pig-Tail/Cert/blob/main/An%20Analysis%20of%20Public%20AWS%20AMI%20Security%20Risks.pdf) · [Azure Pentest Lab (SANS)](https://github.com/Pig-Tail/Cert/blob/main/Azure%20pentest%20lab%20SANS.pdf) · [MCBTA](https://github.com/Pig-Tail/Cert/blob/main/Multi-Cloud%20Threat%20Detection%20Approaches%20Using%20MCBTA.pdf) · [AWS Flow Logs](https://github.com/Pig-Tail/Cert/blob/main/Tux%27s%20Magic%20Hat%20_%20Analysing%20AWS%20Flow%20Logs%20for%20Fun%21.pdf) · [External Attack Surface (AWS)](https://github.com/Pig-Tail/Cert/blob/main/External%20Attack%20Surface%20for%20Initial%20Access%20in%20AWS%20Cloud%20Webinar.pdf) |
| 🌐 **Web / API / Mobile** | [Hacking APIs](https://github.com/Pig-Tail/Cert/blob/main/Hacking%20APIs_%20Web%20API%20Pentesting%20Essentials.pdf) · [Practical Web AppSec & Testing](https://github.com/Pig-Tail/Cert/blob/main/certificate-of-completion-for-practical-web-application-security-and-testing.pdf) · [Mobile App Pentesting](https://github.com/Pig-Tail/Cert/blob/main/certificate-of-completion-for-mobile-application-penetration-testing.pdf) · [Practical Ethical Hacking](https://github.com/Pig-Tail/Cert/blob/main/certificate-of-completion-for-practical-ethical-hacking-the-complete-course.pdf) · [Movement, Pivoting & Persistence](https://github.com/Pig-Tail/Cert/blob/main/certificate-of-completion-for-movement-pivoting-and-persistence-for-pentesters-and-ethical-hackers.pdf) |
| 🏭 **ICS / OT / IoT / Medical** | [210W-07 ICS Vulnerabilities](https://github.com/Pig-Tail/Cert/blob/main/210W-07%20ICS%20Cybersecurity%20Vulnerabilities.pdf) · [210W-09 IT & ICS Attack Methods](https://github.com/Pig-Tail/Cert/blob/main/210W-09%20Attack%20Methodologies%20in%20IT%20%26%20ICS.pdf) · [OT Security](https://github.com/Pig-Tail/Cert/blob/main/certificate-an-introduction-to-ot-security-6569b4be615f9a2c73090266.pdf) · [Medical Device Security](https://github.com/Pig-Tail/Cert/blob/main/certificate-medical-device-security-6576ead7a9a4f0f26a0a1560.pdf) · [IoT Pentesting](https://github.com/Pig-Tail/Cert/blob/main/Introduction%20to%20IoT%20Penetration%20Testing.pdf) |
| 🔵 **Blue / Purple / DFIR / CTI** | [Purple Teaming Fundamentals](https://github.com/Pig-Tail/Cert/blob/main/Purple%20teaming%20fundamentals.pdf) · [CTI (SANS)](https://github.com/Pig-Tail/Cert/blob/main/CTI%20SANS.pdf) · [HELK](https://github.com/Pig-Tail/Cert/blob/main/HELK.pdf) · [MITRE ATT&CK](https://github.com/Pig-Tail/Cert/blob/main/Introducci%C3%B3n%20a%20Mitre.pdf) · [Practical Malware Analysis & Triage](https://github.com/Pig-Tail/Cert/blob/main/certificate-of-completion-for-practical-malware-analysis-triage.pdf) |
| 🤖 **AI Security** | [Claude Computer Use — Prompt Injection to Shells](https://github.com/Pig-Tail/Cert/blob/main/Claude%20Computer%20Use_%20From%20Prompt%20Injection%20to%20Raining%20Shells.pdf) |

<sub>→ full indexed set (58 certificates) in <a href="https://github.com/Pig-Tail/Cert">Pig-Tail/Cert</a>.</sub>

---

<p align="center"><sub>Coordinated disclosure / collaboration → jorge@jmilla.es · <a href="https://twitter.com/jgonzalezmilla">@jgonzalezmilla</a></sub></p>
