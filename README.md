<h1 align="center">Jorge González Milla</h1>
<p align="center"><b><code>Pig-Tail</code></b> · Offensive Security Engineer · Vulnerability Researcher · Red Teamer</p>
<p align="center">
  <img src="https://img.shields.io/badge/Security_Advisories-156+-e5654a?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Critical-9-b5185c?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/High-58-e5654a?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Assigned_CVEs-23-d9822b?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Projects-57+-56b6c2?labelColor=24292f&style=flat-square">
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

| CVE | Project | Vulnerability | Advisory |
|:--|:--|:--|:--|
| **CVE-2026-14620** | `webpack-dev-server` | webpack-dev-server vulnerable to cross-site request forgery via intern | [`GHSA-f5vj-f2hx-8m93`](https://github.com/webpack/webpack-dev-server/security/advisories/GHSA-f5vj-f2hx-8m93) |
| **CVE-2026-40936** | `glpi-agent` | ToolBox plugin can allow unauthenticated path traversal leading to arb | [`GHSA-5379-v7xc-36m8`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-5379-v7xc-36m8) |
| **CVE-2026-42187** | `glpi-agent` | Proxy plugin can allow arbitrary file write if `local_store` is enable | [`GHSA-2w23-rj57-xq9c`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-2w23-rj57-xq9c) |
| **CVE-2026-45621** | `glpi-agent` | MongoDB inventory module allows JavaScript injection via unescaped log | [`GHSA-xqcp-72qc-36p2`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-xqcp-72qc-36p2) |
| **CVE-2026-46615** | `glpi-agent` | Database inventory modules execute OS commands with unsanitized databa | [`GHSA-fcgf-g6c2-g838`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-fcgf-g6c2-g838) |
| **CVE-2026-48728** | `glpi-inventory-plugin` | Job enumeration and status manipulation on Deploy, Collect, and ESX ag | [`GHSA-xj72-9f7x-f4hm`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-xj72-9f7x-f4hm) |
| **CVE-2026-48730** | `glpi-inventory-plugin` | Reflected XSS | [`GHSA-97vv-hxvv-9rw8`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-97vv-hxvv-9rw8) |
| **CVE-2026-49285** | `glpi-agent` | OS Command Injection in GLPI Agent ToolBox Results export via unsaniti | [`GHSA-3974-4pff-75wp`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-3974-4pff-75wp) |
| **CVE-2026-52764** | `glpi-agent` | MSSQL inventory module executes OS commands with unsanitized database  | [`GHSA-r9rr-vpw9-p66x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-r9rr-vpw9-p66x) |
| **CVE-2026-52765** | `glpi-agent` | Oracle and DB2 inventory modules allow SQL injection in GLPI server-su | [`GHSA-4px8-6x8g-722x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-4px8-6x8g-722x) |
| **CVE-2026-52768** | `glpi-agent` | Deploy task Path Traversal in Tools::Archive | [`GHSA-g2f7-8mp5-qw65`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-g2f7-8mp5-qw65) |
| **CVE-2026-53626** | `glpi` | Arbitrary document read | [`GHSA-q9rc-v6vm-q5mm`](https://github.com/glpi-project/glpi/security/advisories/GHSA-q9rc-v6vm-q5mm) |
| **CVE-2026-54697** | `cbssh` | Excessive allocation and integer overflow in DER private-key parsing | [`GHSA-vc8p-8pxg-rfwg`](https://github.com/connectbot/cbssh/security/advisories/GHSA-vc8p-8pxg-rfwg) |
| **CVE-2026-54764** | `traefik` | ForwardAuth middleware leaks X-Forwarded-Port spoofing via untrusted X | [`GHSA-3q9r-p662-5j8m`](https://github.com/traefik/traefik/security/advisories/GHSA-3q9r-p662-5j8m) |
| **CVE-2026-55422** | `conda-forge` | Stored DOM XSS on conda-forge.org via unsanitized dangerouslySetInnerH | [`GHSA-r5vj-wgjv-r524`](https://github.com/conda-forge/conda-forge.github.io/security/advisories/GHSA-r5vj-wgjv-r524) |
| **CVE-2026-55780** | `NanaZip` | Uncaught exception / unbounded allocation in NanaZip .NET single-file  | [`GHSA-ppm9-5267-rq72`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-ppm9-5267-rq72) |
| **CVE-2026-55781** | `NanaZip` | Unbounded memory allocation (DoS) in NanaZip UFS parser via unvalidate | [`GHSA-m34h-jf84-m74h`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-m34h-jf84-m74h) |
| **CVE-2026-55782** | `NanaZip` | Unbounded memory allocation (DoS) in NanaZip WebAssembly parser via at | [`GHSA-qxhc-2v6p-wm8m`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-qxhc-2v6p-wm8m) |
| **CVE-2026-55783** | `NanaZip` | NULL pointer dereference in Extract() of all seven NanaZip custom arch | [`GHSA-q67r-9cfh-xc29`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-q67r-9cfh-xc29) |
| **CVE-2026-57562** | `readest` | Subscription/entitlement hijack: /api/stripe/check binds any paid Chec | [`GHSA-pv88-3727-j7v8`](https://github.com/readest/readest/security/advisories/GHSA-pv88-3727-j7v8) |
| **CVE-2026-57565** | `readest` | Cross-tenant object write via unsanitized fileName in /api/storage/upl | [`GHSA-mfmj-2frf-vhgw`](https://github.com/readest/readest/security/advisories/GHSA-mfmj-2frf-vhgw) |
| **CVE-2026-57566** | `readest` | Unauthenticated SSRF / open request proxy in /api/opds/proxy | [`GHSA-c7mm-g2j2-98cx`](https://github.com/readest/readest/security/advisories/GHSA-c7mm-g2j2-98cx) |
| **CVE-2026-57567** | `readest` | Unscoped Tauri IPC download_file/upload_file allow arbitrary local fil | [`GHSA-55vr-pvq5-6fmg`](https://github.com/readest/readest/security/advisories/GHSA-55vr-pvq5-6fmg) |

---

### 🐛 All security advisories

**156+ advisories** across **57 projects** · **9 Critical · 58 High · 68 Medium · 21 Low**
<sub>(verified from GitHub Security Advisories credited to <code>Pig-Tail</code>; coordinated disclosure)</sub>

#### 🔴 Critical
| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `cbssh` | Server-Side Request Forgery (SSRF) via Unrestricted SOCKS5 Dynamic Port Forwarding | CWE-918 | [`GHSA-4q4j-9h6q-3qr8`](https://github.com/connectbot/cbssh/security/advisories/GHSA-4q4j-9h6q-3qr8) |
| `dbgate` | Unauthenticated RCE via /plugins/command and /plugins/auth-types arbitrary module  | CWE-94/CWE-306/CWE-829 | [`GHSA-2h9g-7xh4-r782`](https://github.com/dbgate/dbgate/security/advisories/GHSA-2h9g-7xh4-r782) |
| `dbgate` | Unauthenticated arbitrary file write via /files/export-diagram-png (and export sib | CWE-22/CWE-73/CWE-94 | [`GHSA-7hjr-q3j2-p5f6`](https://github.com/dbgate/dbgate/security/advisories/GHSA-7hjr-q3j2-p5f6) |
| `dbgate` | Unauthenticated arbitrary file write (RCE) via jsldata saveText/saveRows file:// j | CWE-22/CWE-73/CWE-306 | [`GHSA-7hp4-h6ch-pcm4`](https://github.com/dbgate/dbgate/security/advisories/GHSA-7hp4-h6ch-pcm4) |
| `dbgate` | Unauthenticated RCE via jsldata.extractTimelineChart -> requirePluginFunction arbi | CWE-94/CWE-95/CWE-306 | [`GHSA-wrfj-crc3-qcw6`](https://github.com/dbgate/dbgate/security/advisories/GHSA-wrfj-crc3-qcw6) |
| `lemmy` | SSRF via Image Proxy in Markdown Processing | CWE-918 | [`GHSA-wfhv-j3cm-8jjf`](https://github.com/LemmyNet/lemmy/security/advisories/GHSA-wfhv-j3cm-8jjf) |
| `openemr` | Unauthenticated Database Schema Upgrade Without CSRF Protection in sql_upgrade.php | CWE-306/CWE-352 | [`GHSA-6m85-6m7m-5jqp`](https://github.com/openemr/openemr/security/advisories/GHSA-6m85-6m7m-5jqp) |
| `openemr` | Unauthenticated SQL Patch Execution via sql_patch.php | CWE-306 | [`GHSA-whgc-4r34-vj3q`](https://github.com/openemr/openemr/security/advisories/GHSA-whgc-4r34-vj3q) |
| `pimcore` | Missing Authorization on element Version mutation/deletion (IDOR): any backend use | CWE-639/CWE-862 | [`GHSA-34vf-ww58-w3wc`](https://github.com/pimcore/pimcore/security/advisories/GHSA-34vf-ww58-w3wc) |

<details><summary>🟠 <b>High</b> (58)</summary>

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `avo` | Missing authorization in Avo Media Library endpoints lets any authenticated user r | CWE-639/CWE-862 | [`GHSA-578q-wf95-rrvv`](https://github.com/avo-hq/avo/security/advisories/GHSA-578q-wf95-rrvv) |
| `avo` | Unauthenticated persistent DoS: unvalidated set_locale param mutates Avo's process | CWE-20/CWE-913 | [`GHSA-w44g-92xf-4mq3`](https://github.com/avo-hq/avo/security/advisories/GHSA-w44g-92xf-4mq3) |
| `budibase` | Chat-app AI agents fail open on access control (unset roleId => all roles) and exe | CWE-276/CWE-862 | [`GHSA-hc6c-rm2j-ch7q`](https://github.com/Budibase/budibase/security/advisories/GHSA-hc6c-rm2j-ch7q) |
| `cbssh` | CPU Exhaustion Denial of Service via Zlib Decompression Bomb | CWE-770 | [`GHSA-47hp-5frr-63c9`](https://github.com/connectbot/cbssh/security/advisories/GHSA-47hp-5frr-63c9) |
| `crate` | X-Real-Ip loopback blacklist is string-based and bypassable -> HBA trust/_local_ m | CWE-290/CWE-348 | [`GHSA-7hv8-vvg6-qx5q`](https://github.com/crate/crate/security/advisories/GHSA-7hv8-vvg6-qx5q) |
| `crate` | Incomplete fix of CVE-2024-24565: case-varied FILE:// scheme bypasses the COPY FRO | CWE-22/CWE-178 | [`GHSA-xw2x-w5xq-9w8r`](https://github.com/crate/crate/security/advisories/GHSA-xw2x-w5xq-9w8r) |
| `dbgate` | SQL injection in database structure analyser via composite database parameter (=SC | CWE-89 | [`GHSA-426j-wrmq-2746`](https://github.com/dbgate/dbgate/security/advisories/GHSA-426j-wrmq-2746) |
| `dbgate` | Hardcoded static JWT secret allows bypassing query permission/RBAC checks in sessi | CWE-285/CWE-639/CWE-798 | [`GHSA-5qrh-34cm-wwqm`](https://github.com/dbgate/dbgate/security/advisories/GHSA-5qrh-34cm-wwqm) |
| `dbgate` | SQL injection via unescaped identifiers (quoteIdentifier does not double the delim | CWE-89 | [`GHSA-984f-46q6-gc5q`](https://github.com/dbgate/dbgate/security/advisories/GHSA-984f-46q6-gc5q) |
| `dbgate` | Unauthenticated SSRF with response exfiltration and arbitrary file read via /files | CWE-22/CWE-918 | [`GHSA-p8jg-4h9w-gxp4`](https://github.com/dbgate/dbgate/security/advisories/GHSA-p8jg-4h9w-gxp4) |
| `fhir-core` | Unauthenticated SSRF via SMART Health Link/Card retrieval during FHIR validation f | CWE-918 | [`GHSA-75qq-wq7q-r8x2`](https://github.com/hapifhir/org.hl7.fhir.core/security/advisories/GHSA-75qq-wq7q-r8x2) |
| `fleet` | Path traversal in helm.valuesFiles (generateValues) enables arbitrary YAML file re | CWE-22 | [`GHSA-4jw9-w8c5-8563`](https://github.com/rancher/fleet/security/advisories/GHSA-4jw9-w8c5-8563) |
| `fleet` | Cross-cluster identity takeover via unauthenticated ClientID claim in ClusterRegis | CWE-290/CWE-863 | [`GHSA-55mc-9jwh-vqcx`](https://github.com/rancher/fleet/security/advisories/GHSA-55mc-9jwh-vqcx) |
| `fleet` | Cross-tenant BundleDeployment/secret disclosure via spoofed agent cluster labels ( | CWE-290/CWE-639 | [`GHSA-6x76-fmmf-99gm`](https://github.com/rancher/fleet/security/advisories/GHSA-6x76-fmmf-99gm) |
| `form-data` | CRLF injection in form-data via unescaped multipart Content-Type (incomplete fix o | CWE-93 | [`GHSA-xmxw-787q-7h3h`](https://github.com/form-data/form-data/security/advisories/GHSA-xmxw-787q-7h3h) |
| `glpi` | Arbitrary document read | CWE-639/CWE-862 | [`GHSA-q9rc-v6vm-q5mm`](https://github.com/glpi-project/glpi/security/advisories/GHSA-q9rc-v6vm-q5mm) · CVE-2026-53626 |
| `glpi-agent` | OS Command Injection in GLPI Agent ToolBox Results export via unsanitized tag_filt | CWE-78 | [`GHSA-3974-4pff-75wp`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-3974-4pff-75wp) · CVE-2026-49285 |
| `glpi-agent` | ToolBox plugin can allow unauthenticated path traversal leading to arbitrary file  | CWE-22/CWE-73 | [`GHSA-5379-v7xc-36m8`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-5379-v7xc-36m8) · CVE-2026-40936 |
| `glpi-agent` | Database inventory modules execute OS commands with unsanitized database names fro | CWE-78 | [`GHSA-fcgf-g6c2-g838`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-fcgf-g6c2-g838) · CVE-2026-46615 |
| `glpi-agent` | MSSQL inventory module executes OS commands with unsanitized database names and cr | CWE-78 | [`GHSA-r9rr-vpw9-p66x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-r9rr-vpw9-p66x) · CVE-2026-52764 |
| `glpi-agent` | MongoDB inventory module allows JavaScript injection via unescaped login credentia | CWE-94/CWE-116 | [`GHSA-xqcp-72qc-36p2`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-xqcp-72qc-36p2) · CVE-2026-45621 |
| `glpi-inventory-plugin` | Reflected XSS | CWE-79 | [`GHSA-97vv-hxvv-9rw8`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-97vv-hxvv-9rw8) · CVE-2026-48730 |
| `grav` | Incomplete fix of GHSA-f8v5: cleanDangerousTwig read_file denylist bypassable via  | CWE-22/CWE-184 | [`GHSA-358m-8xgp-rchr`](https://github.com/getgrav/grav/security/advisories/GHSA-358m-8xgp-rchr) |
| `hono` | CSS rule injection via interpolated string values in the hono/css template helper  | CWE-74/CWE-79 | [`GHSA-c9w3-vxph-34px`](https://github.com/honojs/hono/security/advisories/GHSA-c9w3-vxph-34px) |
| `horilla-hr` | Authentication Bypass in Protected Media Endpoint via HTTP Referer Header Allows U | CWE-290/CWE-639 | [`GHSA-rx36-x4qw-v5cp`](https://github.com/horilla/horilla-hr/security/advisories/GHSA-rx36-x4qw-v5cp) |
| `kirby` | Unauthenticated Panel installation via spoofable Host-suffix isLocal() shortcut (i | CWE-290/CWE-1188 | [`GHSA-x399-9qhw-fprv`](https://github.com/getkirby/kirby/security/advisories/GHSA-x399-9qhw-fprv) |
| `lemmy` | Domain-Based Trust Bypass in verify_mod_action Allows Unauthorized Moderation Acti | CWE-284 | [`GHSA-38f7-ccrg-ccmf`](https://github.com/LemmyNet/lemmy/security/advisories/GHSA-38f7-ccrg-ccmf) |
| `nebula-mesh` | Certificate revocation is never enforced at the mesh: nebula-agent drops the polle | CWE-299/CWE-672 | [`GHSA-cm26-5974-52h8`](https://github.com/forgekeep/nebula-mesh/security/advisories/GHSA-cm26-5974-52h8) |
| `netty-incubator-codec-ohttp` | BinaryHttpParser: Unauthenticated CPU-exhaustion DoS via infinite loop in field-se | CWE-400/CWE-835 | [`GHSA-4899-mpch-38p3`](https://github.com/netty/netty-incubator-codec-ohttp/security/advisories/GHSA-4899-mpch-38p3) |
| `nocodb` | Public shared-view row-filter bypass: unauthenticated read of filtered-out rows' l | CWE-639/CWE-863 | [`GHSA-xjxh-mq5w-mpq6`](https://github.com/nocodb/nocodb/security/advisories/GHSA-xjxh-mq5w-mpq6) |
| `nodemailer` | Message-level raw option bypasses disableFileAccess/disableUrlAccess, enabling arb | CWE-73/CWE-918 | [`GHSA-p6gq-j5cr-w38f`](https://github.com/nodemailer/nodemailer/security/advisories/GHSA-p6gq-j5cr-w38f) |
| `OpenAM` | OpenAM WebAuthn Java deserialization RCE via ObjectInputFilter depth | CWE-502 | [`GHSA-gf8h-gq53-288j`](https://github.com/OpenIdentityPlatform/OpenAM/security/advisories/GHSA-gf8h-gq53-288j) |
| `openbabel` | Out-of-bounds write in InChI output writer for atoms with more than 20 bonds (inch | CWE-787 | [`GHSA-9hgq-4w8g-43wj`](https://github.com/openbabel/openbabel/security/advisories/GHSA-9hgq-4w8g-43wj) |
| `opencti` | Unauthenticated resource exhaustion via pre-auth body parsing in TAXII push endpoi | CWE-400 | [`GHSA-6crf-vqpj-hvr4`](https://github.com/OpenCTI-Platform/opencti/security/advisories/GHSA-6crf-vqpj-hvr4) |
| `opencti` | SSRF via response-controlled pagination URL in JSON ingestion feature | CWE-918 | [`GHSA-w3h6-4frq-fgm7`](https://github.com/OpenCTI-Platform/opencti/security/advisories/GHSA-w3h6-4frq-fgm7) |
| `opendj` | OpenDJ Unbounded VLV offset array allocation → memory-exhaustion DoS | CWE-190/CWE-770/CWE-789 | [`GHSA-q4wx-wj4j-4657`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-q4wx-wj4j-4657) |
| `opendj` | OpenDJ Unauthenticated stack exhaustion when decoding an LDAP search filter (DoS) | CWE-400/CWE-674 | [`GHSA-rv4q-c6mr-wxp7`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-rv4q-c6mr-wxp7) |
| `openemr` | Unauthenticated Access Control List Upgrade via acl_upgrade.php | CWE-306 | [`GHSA-gvwm-jrrc-6qqq`](https://github.com/openemr/openemr/security/advisories/GHSA-gvwm-jrrc-6qqq) |
| `Paymenter` | Stripe webhook signature verification fails open on empty secret, enabling unauthe | CWE-345/CWE-347 | [`GHSA-v6g5-fc72-rxg9`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-v6g5-fc72-rxg9) |
| `pimcore` | Incomplete fix of Twig sandbox hardening (#19193 / GHSA-5qxq sibling): model gette | CWE-693/CWE-1336 | [`GHSA-7gfm-v2fx-xrxm`](https://github.com/pimcore/pimcore/security/advisories/GHSA-7gfm-v2fx-xrxm) |
| `pnpm` | Incomplete fix of CVE-2026-55180: repository pnpm-workspace.yaml expands env secre | CWE-201/CWE-522 | [`GHSA-564m-5w64-9vwm`](https://github.com/pnpm/pnpm/security/advisories/GHSA-564m-5w64-9vwm) |
| `posthog` | SSRF Protection Bypass When DEBUG=True | CWE-918 | [`GHSA-hqp7-494m-49v4`](https://github.com/PostHog/posthog/security/advisories/GHSA-hqp7-494m-49v4) |
| `probo` | Server-Side Request Forgery in the third-party vetting agent HTTP tools (analyze_c | CWE-918 | [`GHSA-2vvx-35h4-gvv4`](https://github.com/getprobo/probo/security/advisories/GHSA-2vvx-35h4-gvv4) |
| `probo` | Vertical privilege escalation: an organization ADMIN can mint an OWNER membership  | CWE-269/CWE-863 | [`GHSA-cppp-g98f-gfpp`](https://github.com/getprobo/probo/security/advisories/GHSA-cppp-g98f-gfpp) |
| `probo` | Account takeover via Microsoft OIDC nOAuth: Probo trusts the unverified email clai | CWE-287/CWE-290 | [`GHSA-px7q-g78h-p5qm`](https://github.com/getprobo/probo/security/advisories/GHSA-px7q-g78h-p5qm) |
| `probo` | Account takeover via OIDC login: the continue redirect hands the victim's root-ses | CWE-384/CWE-601 | [`GHSA-r9mf-88r7-g6j9`](https://github.com/getprobo/probo/security/advisories/GHSA-r9mf-88r7-g6j9) |
| `rancher` | Server-Side Request Forgery in catalog HTTP client via attacker-controlled chart i | CWE-918 | [`GHSA-85ph-vjjm-hpcj`](https://github.com/rancher/rancher/security/advisories/GHSA-85ph-vjjm-hpcj) |
| `rancher` | Ownership-less ClusterRole overwrite via attacker-controlled cr-name annotation on | CWE-269/CWE-284 | [`GHSA-9pww-5546-rq68`](https://github.com/rancher/rancher/security/advisories/GHSA-9pww-5546-rq68) |
| `readest` | Unscoped Tauri IPC download_file/upload_file allow arbitrary local file write and  | CWE-22 | [`GHSA-55vr-pvq5-6fmg`](https://github.com/readest/readest/security/advisories/GHSA-55vr-pvq5-6fmg) · CVE-2026-57567 |
| `readest` | Unauthenticated SSRF / open request proxy in /api/opds/proxy | CWE-918 | [`GHSA-c7mm-g2j2-98cx`](https://github.com/readest/readest/security/advisories/GHSA-c7mm-g2j2-98cx) · CVE-2026-57566 |
| `readest` | Cross-tenant object write via unsanitized fileName in /api/storage/upload (object- | CWE-22 | [`GHSA-mfmj-2frf-vhgw`](https://github.com/readest/readest/security/advisories/GHSA-mfmj-2frf-vhgw) · CVE-2026-57565 |
| `readest` | Subscription/entitlement hijack: /api/stripe/check binds any paid Checkout Session | CWE-639 | [`GHSA-pv88-3727-j7v8`](https://github.com/readest/readest/security/advisories/GHSA-pv88-3727-j7v8) · CVE-2026-57562 |
| `shopper` | Missing authorization on product variant DeleteAction/DeleteBulkAction in Form\\Va | CWE-285/CWE-862 | [`GHSA-93v2-gcw2-vfwc`](https://github.com/shopperlabs/shopper/security/advisories/GHSA-93v2-gcw2-vfwc) |
| `signalk-server` | Path Traversal in built-in File Resource Provider → arbitrary JSON file read (secu | CWE-22 | [`GHSA-9xw6-rr23-hg92`](https://github.com/SignalK/signalk-server/security/advisories/GHSA-9xw6-rr23-hg92) |
| `surrealdb` | SSRF via HTTP Redirect Following in HTTP Functions | CWE-918 | [`GHSA-qcm8-xfx5-m6x7`](https://github.com/surrealdb/surrealdb/security/advisories/GHSA-qcm8-xfx5-m6x7) |
| `traefik` | Denial of Service via externally injectable X-Traefik-Router header in DenyRouterR | CWE-400 | [`GHSA-pmf8-jgrq-wm4x`](https://github.com/traefik/traefik/security/advisories/GHSA-pmf8-jgrq-wm4x) |
| `traefik` | PassTLSClientCert middleware does not strip X-Forwarded-Tls-Client-Cert when no mT | CWE-287 | [`GHSA-rmwc-695g-cq94`](https://github.com/traefik/traefik/security/advisories/GHSA-rmwc-695g-cq94) |
| `xwiki-pro-macros` | Stored XSS via unescaped color parameter in the Button macro (incomplete fix of th | CWE-79 | [`GHSA-2h32-52j5-qg3h`](https://github.com/xwikisas/xwiki-pro-macros/security/advisories/GHSA-2h32-52j5-qg3h) |

</details>

<details><summary>🟡 <b>Medium</b> (68)</summary>

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `actual` | Persistent multi-user sync denial-of-service via unvalidated CRDT dataset/column i | CWE-20/CWE-400 | [`GHSA-fpqg-7f23-v2qm`](https://github.com/actualbudget/actual/security/advisories/GHSA-fpqg-7f23-v2qm) |
| `angular` | platform-server validateAllowedHosts fails open for non-absolute URLs — host allow | CWE-636/CWE-918 | [`GHSA-4xvg-mpqx-2jmg`](https://github.com/angular/angular/security/advisories/GHSA-4xvg-mpqx-2jmg) |
| `authelia` | Missing elevated-session (step-up) authorization on TOTP deletion lets a password- | CWE-862 | [`GHSA-6849-pcxw-x2cx`](https://github.com/authelia/authelia/security/advisories/GHSA-6849-pcxw-x2cx) |
| `authelia` | Access control bypass: authenticated {user}/{group} domain rules matched case-sens | CWE-178/CWE-863 | [`GHSA-7w46-9qgm-wgfw`](https://github.com/authelia/authelia/security/advisories/GHSA-7w46-9qgm-wgfw) |
| `cbssh` | Insufficient DH Group Validation in Diffie-Hellman Group Exchange | CWE-325 | [`GHSA-h8g5-x45x-3w25`](https://github.com/connectbot/cbssh/security/advisories/GHSA-h8g5-x45x-3w25) |
| `cbssh` | Excessive allocation and integer overflow in DER private-key parsing | CWE-190/CWE-789 | [`GHSA-vc8p-8pxg-rfwg`](https://github.com/connectbot/cbssh/security/advisories/GHSA-vc8p-8pxg-rfwg) · CVE-2026-54697 |
| `centrifugo` | gRPC server API silently fails open (unauthenticated) when enabled without a key ( | CWE-306/CWE-1188 | [`GHSA-968h-5v87-f62f`](https://github.com/centrifugal/centrifugo/security/advisories/GHSA-968h-5v87-f62f) |
| `conda-forge` | Stored DOM XSS on conda-forge.org via unsanitized dangerouslySetInnerHTML in the s | CWE-79 | [`GHSA-r5vj-wgjv-r524`](https://github.com/conda-forge/conda-forge.github.io/security/advisories/GHSA-r5vj-wgjv-r524) · CVE-2026-55422 |
| `crate` | PostgreSQL wire Bind: attacker-controlled parameter length drives unbounded byte[] | CWE-789/CWE-1284 | [`GHSA-4r2j-q62w-2r4f`](https://github.com/crate/crate/security/advisories/GHSA-4r2j-q62w-2r4f) |
| `crate` | HTTP auth handler caches authorized user per connection and skips credential re-va | CWE-287 | [`GHSA-8jr8-9wjf-7m2h`](https://github.com/crate/crate/security/advisories/GHSA-8jr8-9wjf-7m2h) |
| `crate` | SSRF: COPY FROM 'http(s)://…' reachable by any low-privilege DML user with no host | CWE-918 | [`GHSA-pfv7-m2fh-6g4v`](https://github.com/crate/crate/security/advisories/GHSA-pfv7-m2fh-6g4v) |
| `directus` | Share token can read sibling items through recursive relation permission derivatio | CWE-639 | [`GHSA-pqp8-63c5-fm34`](https://github.com/directus/directus/security/advisories/GHSA-pqp8-63c5-fm34) |
| `fhir-core` | Unauthenticated SSRF via /txTest endpoint (server parameter) of the FHIR Validator | CWE-918 | [`GHSA-c3w2-qwwp-ww4h`](https://github.com/hapifhir/org.hl7.fhir.core/security/advisories/GHSA-c3w2-qwwp-ww4h) |
| `fleet` | Unauthenticated cross-namespace GitRepo Spec/Status mutation via git webhook recei | CWE-306/CWE-862 | [`GHSA-qhgf-p2mp-2r94`](https://github.com/rancher/fleet/security/advisories/GHSA-qhgf-p2mp-2r94) |
| `glances` | Incomplete fix of CORS wildcard+credentials guard: reflected-origin with credentia | CWE-346/CWE-942 | [`GHSA-q39q-mvj4-gp24`](https://github.com/nicolargo/glances/security/advisories/GHSA-q39q-mvj4-gp24) |
| `glpi-agent` | Proxy plugin can allow arbitrary file write if `local_store` is enabled | CWE-22 | [`GHSA-2w23-rj57-xq9c`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-2w23-rj57-xq9c) · CVE-2026-42187 |
| `glpi-agent` | Oracle and DB2 inventory modules allow SQL injection in GLPI server-supplied crede | CWE-89 | [`GHSA-4px8-6x8g-722x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-4px8-6x8g-722x) · CVE-2026-52765 |
| `glpi-agent` | OS Command Injection via server-controlled archive filename in Deploy task | CWE-78 | [`GHSA-fh99-rgmp-c623`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-fh99-rgmp-c623) |
| `glpi-agent` | Deploy task Path Traversal in Tools::Archive | CWE-22/CWE-23 | [`GHSA-g2f7-8mp5-qw65`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-g2f7-8mp5-qw65) · CVE-2026-52768 |
| `glpi-agent` | glpi-agent ToolBox: Unauthenticated SNMP network scanning against arbitrary IP ran | CWE-284/CWE-918 | [`GHSA-vv6x-8qfx-x756`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-vv6x-8qfx-x756) |
| `glpi-inventory-plugin` | Missing SQL escaping in LIKE query allows potential SQL injection when searching d | CWE-89/CWE-116 | [`GHSA-8h4x-cpp3-2qc8`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-8h4x-cpp3-2qc8) |
| `glpi-inventory-plugin` | Job enumeration and status manipulation on Deploy, Collect, and ESX agent API endp | CWE-306 | [`GHSA-xj72-9f7x-f4hm`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-xj72-9f7x-f4hm) · CVE-2026-48728 |
| `gogs` | Unbounded memory allocation in Git LFS batch API enables denial of service | CWE-400/CWE-770 | [`GHSA-m8mh-w9hx-mmjm`](https://github.com/gogs/gogs/security/advisories/GHSA-m8mh-w9hx-mmjm) |
| `gogs` | Image decompression bomb in avatar upload enables denial of service | CWE-400/CWE-409 | [`GHSA-v5vf-9g9p-p9fg`](https://github.com/gogs/gogs/security/advisories/GHSA-v5vf-9g9p-p9fg) |
| `gonic` | Incomplete fix of CVE-2026-49338: getCoverArt for playlists lacks the ownership ch | CWE-639/CWE-862 | [`GHSA-364r-g89f-rmg3`](https://github.com/sentriz/gonic/security/advisories/GHSA-364r-g89f-rmg3) |
| `horilla-hr` | Server-Side Template Injection (SSTI) in Mail Preview Endpoints Allows Authenticat | CWE-94/CWE-200 | [`GHSA-9p83-4w63-7c24`](https://github.com/horilla/horilla-hr/security/advisories/GHSA-9p83-4w63-7c24) |
| `horilla-hr` | IDOR in Template Hint Endpoint Allows Authenticated Users to Read Arbitrary Candid | CWE-284/CWE-639 | [`GHSA-prj3-h3hc-7fv6`](https://github.com/horilla/horilla-hr/security/advisories/GHSA-prj3-h3hc-7fv6) |
| `kirby` | Unauthenticated path traversal in Media::thumb — request filename not contained in | CWE-22 | [`GHSA-9vx2-j98c-p72w`](https://github.com/getkirby/kirby/security/advisories/GHSA-9vx2-j98c-p72w) |
| `monitoring-plugins` | SSRF and Redfish session-token disclosure via unvalidated @odata.id link in redfis | CWE-20/CWE-918 | [`GHSA-96fx-pqc3-28xv`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-96fx-pqc3-28xv) |
| `openbabel` | NULL-pointer dereference in GAMESS-output MOPAC-charges block (gamessformat.cpp) | CWE-476 | [`GHSA-h28m-r6fh-m3vg`](https://github.com/openbabel/openbabel/security/advisories/GHSA-h28m-r6fh-m3vg) |
| `openbabel` | NULL-pointer dereference in Jaguar-output atomic-charge parser (jaguarformat.cpp) | CWE-476 | [`GHSA-hx98-c7vh-jv7f`](https://github.com/openbabel/openbabel/security/advisories/GHSA-hx98-c7vh-jv7f) |
| `openbabel` | NULL-pointer dereference in Gaussian-output NMR-shift block (gaussformat.cpp) | CWE-476 | [`GHSA-jq53-w56h-97vp`](https://github.com/openbabel/openbabel/security/advisories/GHSA-jq53-w56h-97vp) |
| `openbabel` | NULL-pointer dereference in COF reader formalq handler (cofformat.cpp) | CWE-476 | [`GHSA-prrc-wr67-3q59`](https://github.com/openbabel/openbabel/security/advisories/GHSA-prrc-wr67-3q59) |
| `openbabel` | NULL-pointer/out-of-bounds dereference in WLN ring parser new_cycle (wln-nextmove. | CWE-476 | [`GHSA-rfj6-35p6-w6gm`](https://github.com/openbabel/openbabel/security/advisories/GHSA-rfj6-35p6-w6gm) |
| `openbao` | CEL programs are compiled and evaluated on every request over attacker-influenced  | CWE-400/CWE-1050 | [`GHSA-j4q2-pjgv-8m5h`](https://github.com/openbao/openbao/security/advisories/GHSA-j4q2-pjgv-8m5h) |
| `openbao` | CEL-based JWT login trusts a program-supplied identity EntityID without alias reso | CWE-290/CWE-863 | [`GHSA-rg8x-cg52-32m5`](https://github.com/openbao/openbao/security/advisories/GHSA-rg8x-cg52-32m5) |
| `opencti` | SSRF via webhook notifier allows authenticated users to reach internal services | CWE-918 | [`GHSA-5gxq-gqvj-wccm`](https://github.com/OpenCTI-Platform/opencti/security/advisories/GHSA-5gxq-gqvj-wccm) |
| `opencti` | CSV injection in rolling CSV feed export (/feeds/:id) via entity-controlled attrib | CWE-1236 | [`GHSA-g354-5h4h-w4vg`](https://github.com/OpenCTI-Platform/opencti/security/advisories/GHSA-g354-5h4h-w4vg) |
| `opencti` | Privilege escalation: read-only KNOWLEDGE user can delete other users' draft works | CWE-285/CWE-862 | [`GHSA-j2p5-vc4m-xxhx`](https://github.com/OpenCTI-Platform/opencti/security/advisories/GHSA-j2p5-vc4m-xxhx) |
| `opendj` | OpenDJ JMX MBean-argument deserialization without a serial filter | CWE-502 | [`GHSA-qj63-3vrg-vcfx`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-qj63-3vrg-vcfx) |
| `openemr` | Missing ACL Check on document_category Controller Allows Any Authenticated User to | CWE-862 | [`GHSA-h93m-g539-4m65`](https://github.com/openemr/openemr/security/advisories/GHSA-h93m-g539-4m65) |
| `openemr` | Unauthenticated Information Disclosure in admin.php Exposes Database Names and Ver | CWE-200/CWE-306 | [`GHSA-q366-cv5v-83w8`](https://github.com/openemr/openemr/security/advisories/GHSA-q366-cv5v-83w8) |
| `openproject` | Content Security Policy allows unsafe-inline styles, weakening XSS defenses | CWE-79/CWE-116 | [`GHSA-h483-xmqh-656j`](https://github.com/opf/openproject/security/advisories/GHSA-h483-xmqh-656j) |
| `openstreetmap-website` | No server-side rate limit on unauthenticated Notes API (note/comment spam + email  | CWE-602/CWE-770 | [`GHSA-cx4c-mgj3-h7fc`](https://github.com/openstreetmap/openstreetmap-website/security/advisories/GHSA-cx4c-mgj3-h7fc) |
| `openstreetmap-website` | GPX trace archive decompression bomb causes memory-exhaustion DoS of the trace-imp | CWE-400/CWE-409 | [`GHSA-g99w-vhvj-jqw4`](https://github.com/openstreetmap/openstreetmap-website/security/advisories/GHSA-g99w-vhvj-jqw4) |
| `otel-ebpf` | Unprivileged DoS via unbounded string scan in .eh_frame CIE parsing crashes the eB | CWE-125 | [`GHSA-f59j-4758-2r6v`](https://github.com/open-telemetry/opentelemetry-ebpf-profiler/security/advisories/GHSA-f59j-4758-2r6v) |
| `otel-ebpf` | Unprivileged DoS via unbounded string scan in .eh_frame CIE parsing crashes the eB | CWE-125 | [`GHSA-q339-h695-fwmv`](https://github.com/open-telemetry/opentelemetry-ebpf-profiler/security/advisories/GHSA-q339-h695-fwmv) |
| `otel-ebpf` | Unprivileged DoS via cyclic NestedClass metadata in .NET PE parsing (infinite loop | CWE-835 | [`GHSA-q99m-mcfv-2m95`](https://github.com/open-telemetry/opentelemetry-ebpf-profiler/security/advisories/GHSA-q99m-mcfv-2m95) |
| `otel-ebpf` | Unprivileged DoS via unvalidated numFuncs in .gopclntab parsing (getFuncMapEntry O | CWE-125 | [`GHSA-xfw7-93rw-jvgf`](https://github.com/open-telemetry/opentelemetry-ebpf-profiler/security/advisories/GHSA-xfw7-93rw-jvgf) |
| `Paymenter` | Coupon global max_uses bypass via concurrent checkout race (over-redemption) | CWE-362/CWE-367 | [`GHSA-4527-v9f7-43vr`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-4527-v9f7-43vr) |
| `Paymenter` | Credit-refund double-spend race condition in service downgrade (doUpgrade) | CWE-362 | [`GHSA-5gmm-hjfj-8ff7`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-5gmm-hjfj-8ff7) |
| `posthog` | Unsafe Pickle Deserialization in Auth Token Cache | CWE-502 | [`GHSA-pwpf-22g2-3j34`](https://github.com/PostHog/posthog/security/advisories/GHSA-pwpf-22g2-3j34) |
| `probo` | Broken access control in public e-signature API: any trust-center visitor can comp | CWE-639/CWE-862 | [`GHSA-22xj-f767-ppw6`](https://github.com/getprobo/probo/security/advisories/GHSA-22xj-f767-ppw6) |
| `probo` | Unauthenticated cross-tenant and hidden-item disclosure via Query.node in the publ | CWE-284/CWE-639 | [`GHSA-6h39-vh9x-wj9p`](https://github.com/getprobo/probo/security/advisories/GHSA-6h39-vh9x-wj9p) |
| `probo` | Unauthenticated bypass of the Trust Center NDA gate: anonymous visitors read NDA-g | CWE-306/CWE-862 | [`GHSA-8qwr-vxw8-6wp7`](https://github.com/getprobo/probo/security/advisories/GHSA-8qwr-vxw8-6wp7) |
| `probo` | Stored XSS in the console via unsanitized Markdown (iframe srcdoc) in Organization | CWE-79 | [`GHSA-9fx8-47w4-3vw8`](https://github.com/getprobo/probo/security/advisories/GHSA-9fx8-47w4-3vw8) |
| `probo` | Cross-tenant IDOR via unvalidated FK references | CWE-639 | [`GHSA-c74x-79w6-63jh`](https://github.com/getprobo/probo/security/advisories/GHSA-c74x-79w6-63jh) |
| `probo` | Broken access control: an organization ADMIN can remove members including OWNERs b | CWE-862/CWE-863 | [`GHSA-mwr9-4p55-wqv3`](https://github.com/getprobo/probo/security/advisories/GHSA-mwr9-4p55-wqv3) |
| `probo` | Race condition (write-skew) in the last-active-owner guard: concurrent removals dr | CWE-362/CWE-367 | [`GHSA-r84f-p5r8-ggj5`](https://github.com/getprobo/probo/security/advisories/GHSA-r84f-p5r8-ggj5) |
| `probo` | Unauthenticated cross-tenant and hidden-item disclosure via Query.node in the publ | CWE-284/CWE-639 | [`GHSA-w23w-f7v2-625w`](https://github.com/getprobo/probo/security/advisories/GHSA-w23w-f7v2-625w) |
| `probo` | Stored XSS in the console via unsanitized Markdown (iframe srcdoc) in Organization | CWE-79 | [`GHSA-x23w-93v7-jm24`](https://github.com/getprobo/probo/security/advisories/GHSA-x23w-93v7-jm24) |
| `rancher` | Project resource-quota bypass via negative peer-namespace field.cattle.io/resource | CWE-770/CWE-863 | [`GHSA-gxxh-fqhr-87qc`](https://github.com/rancher/rancher/security/advisories/GHSA-gxxh-fqhr-87qc) |
| `security` | Stored DOM XSS on conda-forge.org via unsanitized dangerouslySetInnerHTML in the s | CWE-79 | [`GHSA-5rxp-7p8x-r93x`](https://github.com/conda-forge/security/security/advisories/GHSA-5rxp-7p8x-r93x) |
| `srvx` | Node adapter URL parser differential: request fragment folded into url.pathname /  | CWE-436 | [`GHSA-ggxm-jf3h-3c2r`](https://github.com/h3js/srvx/security/advisories/GHSA-ggxm-jf3h-3c2r) |
| `statamic` | Missing authorization on navigation endpoint allows disclosure of restricted entri | CWE-639/CWE-862 | [`GHSA-qh8c-7588-qfrv`](https://github.com/statamic/cms/security/advisories/GHSA-qh8c-7588-qfrv) |
| `surrealdb` | SSRF via JWKS URL — Redirect Following in JWT Key Fetch | CWE-918 | [`GHSA-h5rg-8p7f-47g2`](https://github.com/surrealdb/surrealdb/security/advisories/GHSA-h5rg-8p7f-47g2) |
| `traefik` | ForwardAuth middleware leaks X-Forwarded-Port spoofing via untrusted X-Forwarded-P | CWE-345 | [`GHSA-3q9r-p662-5j8m`](https://github.com/traefik/traefik/security/advisories/GHSA-3q9r-p662-5j8m) · CVE-2026-54764 |
| `webpack-dev-server` | webpack-dev-server vulnerable to cross-site request forgery via internal developer | CWE-352/CWE-749 | [`GHSA-f5vj-f2hx-8m93`](https://github.com/webpack/webpack-dev-server/security/advisories/GHSA-f5vj-f2hx-8m93) · CVE-2026-14620 |

</details>

<details><summary>⚪ <b>Low</b> (21)</summary>

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `glpi-agent` | Stored XSS via job tag field in ToolBox Inventory configuration (input/tag) | CWE-79 | [`GHSA-6995-8gmf-q4r2`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-6995-8gmf-q4r2) |
| `glpi-agent` | Stored XSS via SNMP community/authprotocol credential fields in ToolBox plugin | CWE-79 | [`GHSA-cwg9-jj5m-pq4q`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-cwg9-jj5m-pq4q) |
| `glpi-agent` | Stored XSS via inventory tag management in ToolBox plugin | CWE-79 | [`GHSA-m44h-67mc-8fxw`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-m44h-67mc-8fxw) |
| `glpi-agent` | Collect task compiles server-controlled regular expression without validation | CWE-1333 | [`GHSA-mgcf-xgv7-5w4x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-mgcf-xgv7-5w4x) |
| `glpi-agent` | [Deploy] Improper Neutralization of Special Elements used in an OS Command ('OS Co | CWE-78/CWE-345 | [`GHSA-r2hc-w524-5fwh`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-r2hc-w524-5fwh) |
| `glpi-agent` | Oracle inventory module uses unvalidated process username in shell su command | CWE-78 | [`GHSA-vwv6-85p7-mjvc`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-vwv6-85p7-mjvc) |
| `glpi-inventory-plugin` | Authenticated user to delete deployment jobs they do not own | CWE-285/CWE-639 | [`GHSA-985x-m8pc-qmg6`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-985x-m8pc-qmg6) |
| `glpi-inventory-plugin` | Missing checks in some ajax calls | CWE-352 | [`GHSA-j5mr-vccg-pqhw`](https://github.com/glpi-project/glpi-inventory-plugin/security/advisories/GHSA-j5mr-vccg-pqhw) |
| `kirby` | OptionsApi file:// SSRF / local file read via blueprint options.api.url | CWE-441/CWE-918 | [`GHSA-2m4q-xm8w-mpwf`](https://github.com/getkirby/kirby/security/advisories/GHSA-2m4q-xm8w-mpwf) |
| `monitoring-plugins` | logfile: legacy-DB migration follows attacker-planted symlink -> root file overwri | CWE-59/CWE-377 | [`GHSA-w2gg-hx6w-24w3`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-w2gg-hx6w-24w3) |
| `NanaZip` | Unbounded memory allocation (DoS) in NanaZip UFS parser via unvalidated fs_bsize/f | CWE-400/CWE-789 | [`GHSA-m34h-jf84-m74h`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-m34h-jf84-m74h) · CVE-2026-55781 |
| `NanaZip` | Uncaught exception / unbounded allocation in NanaZip .NET single-file Extract() vi | CWE-248/CWE-400 | [`GHSA-ppm9-5267-rq72`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-ppm9-5267-rq72) · CVE-2026-55780 |
| `NanaZip` | NULL pointer dereference in Extract() of all seven NanaZip custom archive handlers | CWE-476 | [`GHSA-q67r-9cfh-xc29`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-q67r-9cfh-xc29) · CVE-2026-55783 |
| `NanaZip` | Unbounded memory allocation (DoS) in NanaZip WebAssembly parser via attacker-contr | CWE-400/CWE-789 | [`GHSA-qxhc-2v6p-wm8m`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-qxhc-2v6p-wm8m) · CVE-2026-55782 |
| `openbao` | Namespace path traversal via URL-encoded '..' in /sys/namespaces/<path> lets a chi | CWE-22 | [`GHSA-26xq-54hr-wmr3`](https://github.com/openbao/openbao/security/advisories/GHSA-26xq-54hr-wmr3) |
| `openemr` | Active Debug Code in fax_view.php Discloses Web Server Group Membership | CWE-200/CWE-489 | [`GHSA-wc2f-fvpv-c32r`](https://github.com/openemr/openemr/security/advisories/GHSA-wc2f-fvpv-c32r) |
| `openproject` | Content Security Policy img-src wildcard enables cross-origin pixel tracking and i | CWE-200 | [`GHSA-m5p8-h274-f7w8`](https://github.com/opf/openproject/security/advisories/GHSA-m5p8-h274-f7w8) |
| `probo` | Consolidated low-severity / hardening findings (plaintext TLS keys, missing auth r | CWE-312/CWE-352/CWE-640/CWE-770 | [`GHSA-7fp4-r448-5v6g`](https://github.com/getprobo/probo/security/advisories/GHSA-7fp4-r448-5v6g) |
| `probo` | Cross-tenant audit-report PDF download via ExportReportPDF missing the trust-cente | CWE-284/CWE-639 | [`GHSA-mrh8-32r4-8hrh`](https://github.com/getprobo/probo/security/advisories/GHSA-mrh8-32r4-8hrh) |
| `traefik` | RedirectScheme middleware trusts untrusted X-Forwarded-Proto header, allowing HTTP | CWE-345 | [`GHSA-q64g-xhfr-vvj2`](https://github.com/traefik/traefik/security/advisories/GHSA-q64g-xhfr-vvj2) |
| `undici` | Insufficient SameSite Cookie Value Validation | CWE-20 | [`GHSA-xvxq-2cc6-x875`](https://github.com/nodejs/undici/security/advisories/GHSA-xvxq-2cc6-x875) |

</details>

---

### 🧰 Tools &amp; research

| Repo | What it is |
|------|------------|
| [alpc-toolkit](https://github.com/Pig-Tail/alpc-toolkit) | Rust toolkit for Windows ALPC/RPC attack-surface recon |
| [Mythic-agent-rust](https://github.com/Pig-Tail/Mythic-agent-rust) | Mythic C2 agent implemented in Rust |
| [HuntingFavicoShodan](https://github.com/Pig-Tail/HuntingFavicoShodan) | Find phishing sites by favicon hash via Shodan |
| [ReconToolTop](https://github.com/Pig-Tail/ReconToolTop) · [Recond_subdomains](https://github.com/Pig-Tail/Recond_subdomains) | Subdomain recon (alive hosts, ports, no API) |
| [Cert](https://github.com/Pig-Tail/Cert) | 📜 Certifications &amp; training (indexed) |

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
