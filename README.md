<h1 align="center">Jorge González Milla</h1>
<p align="center"><b><code>Pig-Tail</code></b> · Offensive Security Engineer · Vulnerability Researcher · Red Teamer</p>
<p align="center">
  <img src="https://img.shields.io/badge/Security_Advisories-79+-e5654a?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Critical-5-e0447b?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Assigned_CVEs-23-d9822b?labelColor=24292f&style=flat-square">
  <img src="https://img.shields.io/badge/Projects-26+-56b6c2?labelColor=24292f&style=flat-square">
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

### 🐛 Security advisories &amp; CVEs

**79 advisories** across **26 projects** · **5 Critical · 34 High · 28 Medium · 12 Low** · **23 assigned CVEs**
<sub>(verified from GitHub Security Advisories credited to <code>Pig-Tail</code>; a subset of the full history since 2017)</sub>

#### 🔴 Critical
| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `dbgate` | Unauthenticated RCE via /plugins/command and /plugins/auth-types arbitrary modul | CWE-94/CWE-306/CWE-829 | [`GHSA-2h9g-7xh4-r782`](https://github.com/dbgate/dbgate/security/advisories/GHSA-2h9g-7xh4-r782) |
| `dbgate` | Unauthenticated arbitrary file write via /files/export-diagram-png (and export s | CWE-22/CWE-73/CWE-94 | [`GHSA-7hjr-q3j2-p5f6`](https://github.com/dbgate/dbgate/security/advisories/GHSA-7hjr-q3j2-p5f6) |
| `dbgate` | Unauthenticated arbitrary file write (RCE) via jsldata saveText/saveRows file:// | CWE-22/CWE-73/CWE-306 | [`GHSA-7hp4-h6ch-pcm4`](https://github.com/dbgate/dbgate/security/advisories/GHSA-7hp4-h6ch-pcm4) |
| `dbgate` | Unauthenticated RCE via jsldata.extractTimelineChart -> requirePluginFunction ar | CWE-94/CWE-95/CWE-306 | [`GHSA-wrfj-crc3-qcw6`](https://github.com/dbgate/dbgate/security/advisories/GHSA-wrfj-crc3-qcw6) |
| `pimcore` | Missing Authorization on element Version mutation/deletion (IDOR): any backend u | CWE-639/CWE-862 | [`GHSA-34vf-ww58-w3wc`](https://github.com/pimcore/pimcore/security/advisories/GHSA-34vf-ww58-w3wc) |

#### 🟠 High
| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `avo` | Missing authorization in Avo Media Library endpoints lets any authenticated user | CWE-639/CWE-862 | [`GHSA-578q-wf95-rrvv`](https://github.com/avo-hq/avo/security/advisories/GHSA-578q-wf95-rrvv) |
| `avo` | Unauthenticated persistent DoS: unvalidated set_locale param mutates Avo's proce | CWE-20/CWE-913 | [`GHSA-w44g-92xf-4mq3`](https://github.com/avo-hq/avo/security/advisories/GHSA-w44g-92xf-4mq3) |
| `crate` | X-Real-Ip loopback blacklist is string-based and bypassable -> HBA trust/_local_ | CWE-290/CWE-348 | [`GHSA-7hv8-vvg6-qx5q`](https://github.com/crate/crate/security/advisories/GHSA-7hv8-vvg6-qx5q) |
| `crate` | Incomplete fix of CVE-2024-24565: case-varied FILE:// scheme bypasses the COPY F | CWE-22/CWE-178 | [`GHSA-xw2x-w5xq-9w8r`](https://github.com/crate/crate/security/advisories/GHSA-xw2x-w5xq-9w8r) |
| `dbgate` | SQL injection in database structure analyser via composite database parameter (= | CWE-89 | [`GHSA-426j-wrmq-2746`](https://github.com/dbgate/dbgate/security/advisories/GHSA-426j-wrmq-2746) |
| `dbgate` | Hardcoded static JWT secret allows bypassing query permission/RBAC checks in ses | CWE-285/CWE-639/CWE-798 | [`GHSA-5qrh-34cm-wwqm`](https://github.com/dbgate/dbgate/security/advisories/GHSA-5qrh-34cm-wwqm) |
| `dbgate` | SQL injection via unescaped identifiers (quoteIdentifier does not double the del | CWE-89 | [`GHSA-984f-46q6-gc5q`](https://github.com/dbgate/dbgate/security/advisories/GHSA-984f-46q6-gc5q) |
| `dbgate` | Unauthenticated SSRF with response exfiltration and arbitrary file read via /fil | CWE-22/CWE-918 | [`GHSA-p8jg-4h9w-gxp4`](https://github.com/dbgate/dbgate/security/advisories/GHSA-p8jg-4h9w-gxp4) |
| `fleet` | Path traversal in helm.valuesFiles (generateValues) enables arbitrary YAML file  | CWE-22 | [`GHSA-4jw9-w8c5-8563`](https://github.com/rancher/fleet/security/advisories/GHSA-4jw9-w8c5-8563) |
| `fleet` | Cross-cluster identity takeover via unauthenticated ClientID claim in ClusterReg | CWE-290/CWE-863 | [`GHSA-55mc-9jwh-vqcx`](https://github.com/rancher/fleet/security/advisories/GHSA-55mc-9jwh-vqcx) |
| `fleet` | Cross-tenant BundleDeployment/secret disclosure via spoofed agent cluster labels | CWE-290/CWE-639 | [`GHSA-6x76-fmmf-99gm`](https://github.com/rancher/fleet/security/advisories/GHSA-6x76-fmmf-99gm) |
| `form-data` | CRLF injection in form-data via unescaped multipart Content-Type (incomplete fix | CWE-93 | [`GHSA-xmxw-787q-7h3h`](https://github.com/form-data/form-data/security/advisories/GHSA-xmxw-787q-7h3h) |
| `glpi-agent` | OS Command Injection in GLPI Agent ToolBox Results export via unsanitized tag_fi | CWE-78 | [`GHSA-3974-4pff-75wp`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-3974-4pff-75wp) · CVE-2026-49285 |
| `glpi-agent` | ToolBox plugin can allow unauthenticated path traversal leading to arbitrary fil | CWE-22/CWE-73 | [`GHSA-5379-v7xc-36m8`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-5379-v7xc-36m8) · CVE-2026-40936 |
| `glpi-agent` | Database inventory modules execute OS commands with unsanitized database names f | CWE-78 | [`GHSA-fcgf-g6c2-g838`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-fcgf-g6c2-g838) · CVE-2026-46615 |
| `glpi-agent` | MSSQL inventory module executes OS commands with unsanitized database names and  | CWE-78 | [`GHSA-r9rr-vpw9-p66x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-r9rr-vpw9-p66x) · CVE-2026-52764 |
| `glpi-agent` | MongoDB inventory module allows JavaScript injection via unescaped login credent | CWE-94/CWE-116 | [`GHSA-xqcp-72qc-36p2`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-xqcp-72qc-36p2) · CVE-2026-45621 |
| `grav` | Incomplete fix of GHSA-f8v5: cleanDangerousTwig read_file denylist bypassable vi | CWE-22/CWE-184 | [`GHSA-358m-8xgp-rchr`](https://github.com/getgrav/grav/security/advisories/GHSA-358m-8xgp-rchr) |
| `hono` | CSS rule injection via interpolated string values in the hono/css template helpe | CWE-74/CWE-79 | [`GHSA-c9w3-vxph-34px`](https://github.com/honojs/hono/security/advisories/GHSA-c9w3-vxph-34px) |
| `kirby` | Unauthenticated Panel installation via spoofable Host-suffix isLocal() shortcut  | CWE-290/CWE-1188 | [`GHSA-x399-9qhw-fprv`](https://github.com/getkirby/kirby/security/advisories/GHSA-x399-9qhw-fprv) |
| `nocodb` | Public shared-view row-filter bypass: unauthenticated read of filtered-out rows' | CWE-639/CWE-863 | [`GHSA-xjxh-mq5w-mpq6`](https://github.com/nocodb/nocodb/security/advisories/GHSA-xjxh-mq5w-mpq6) |
| `openbabel` | Out-of-bounds write in InChI output writer for atoms with more than 20 bonds (in | CWE-787 | [`GHSA-9hgq-4w8g-43wj`](https://github.com/openbabel/openbabel/security/advisories/GHSA-9hgq-4w8g-43wj) |
| `opendj` | OpenDJ Unbounded VLV offset array allocation → memory-exhaustion DoS | CWE-190/CWE-770/CWE-789 | [`GHSA-q4wx-wj4j-4657`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-q4wx-wj4j-4657) |
| `opendj` | OpenDJ Unauthenticated stack exhaustion when decoding an LDAP search filter (DoS | CWE-400/CWE-674 | [`GHSA-rv4q-c6mr-wxp7`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-rv4q-c6mr-wxp7) |
| `Paymenter` | Stripe webhook signature verification fails open on empty secret, enabling unaut | CWE-345/CWE-347 | [`GHSA-v6g5-fc72-rxg9`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-v6g5-fc72-rxg9) |
| `pimcore` | Incomplete fix of Twig sandbox hardening (#19193 / GHSA-5qxq sibling): model get | CWE-693/CWE-1336 | [`GHSA-7gfm-v2fx-xrxm`](https://github.com/pimcore/pimcore/security/advisories/GHSA-7gfm-v2fx-xrxm) |
| `pnpm` | Incomplete fix of CVE-2026-55180: repository pnpm-workspace.yaml expands env sec | CWE-201/CWE-522 | [`GHSA-564m-5w64-9vwm`](https://github.com/pnpm/pnpm/security/advisories/GHSA-564m-5w64-9vwm) |
| `rancher` | Server-Side Request Forgery in catalog HTTP client via attacker-controlled chart | CWE-918 | [`GHSA-85ph-vjjm-hpcj`](https://github.com/rancher/rancher/security/advisories/GHSA-85ph-vjjm-hpcj) |
| `rancher` | Ownership-less ClusterRole overwrite via attacker-controlled cr-name annotation  | CWE-269/CWE-284 | [`GHSA-9pww-5546-rq68`](https://github.com/rancher/rancher/security/advisories/GHSA-9pww-5546-rq68) |
| `readest` | Unscoped Tauri IPC download_file/upload_file allow arbitrary local file write an | CWE-22 | [`GHSA-55vr-pvq5-6fmg`](https://github.com/readest/readest/security/advisories/GHSA-55vr-pvq5-6fmg) · CVE-2026-57567 |
| `readest` | Unauthenticated SSRF / open request proxy in /api/opds/proxy | CWE-918 | [`GHSA-c7mm-g2j2-98cx`](https://github.com/readest/readest/security/advisories/GHSA-c7mm-g2j2-98cx) · CVE-2026-57566 |
| `readest` | Cross-tenant object write via unsanitized fileName in /api/storage/upload (objec | CWE-22 | [`GHSA-mfmj-2frf-vhgw`](https://github.com/readest/readest/security/advisories/GHSA-mfmj-2frf-vhgw) · CVE-2026-57565 |
| `readest` | Subscription/entitlement hijack: /api/stripe/check binds any paid Checkout Sessi | CWE-639 | [`GHSA-pv88-3727-j7v8`](https://github.com/readest/readest/security/advisories/GHSA-pv88-3727-j7v8) · CVE-2026-57562 |
| `signalk-server` | Path Traversal in built-in File Resource Provider → arbitrary JSON file read (se | CWE-22 | [`GHSA-9xw6-rr23-hg92`](https://github.com/SignalK/signalk-server/security/advisories/GHSA-9xw6-rr23-hg92) |

<details><summary>🟡 <b>Medium</b> (28)</summary>

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `centrifugo` | gRPC server API silently fails open (unauthenticated) when enabled without a key | CWE-306/CWE-1188 | [`GHSA-968h-5v87-f62f`](https://github.com/centrifugal/centrifugo/security/advisories/GHSA-968h-5v87-f62f) |
| `crate` | PostgreSQL wire Bind: attacker-controlled parameter length drives unbounded byte | CWE-789/CWE-1284 | [`GHSA-4r2j-q62w-2r4f`](https://github.com/crate/crate/security/advisories/GHSA-4r2j-q62w-2r4f) |
| `crate` | HTTP auth handler caches authorized user per connection and skips credential re- | CWE-287 | [`GHSA-8jr8-9wjf-7m2h`](https://github.com/crate/crate/security/advisories/GHSA-8jr8-9wjf-7m2h) |
| `crate` | SSRF: COPY FROM 'http(s)://…' reachable by any low-privilege DML user with no ho | CWE-918 | [`GHSA-pfv7-m2fh-6g4v`](https://github.com/crate/crate/security/advisories/GHSA-pfv7-m2fh-6g4v) |
| `fleet` | Unauthenticated cross-namespace GitRepo Spec/Status mutation via git webhook rec | CWE-306/CWE-862 | [`GHSA-qhgf-p2mp-2r94`](https://github.com/rancher/fleet/security/advisories/GHSA-qhgf-p2mp-2r94) |
| `glpi-agent` | Proxy plugin can allow arbitrary file write if `local_store` is enabled | CWE-22 | [`GHSA-2w23-rj57-xq9c`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-2w23-rj57-xq9c) · CVE-2026-42187 |
| `glpi-agent` | Oracle and DB2 inventory modules allow SQL injection in GLPI server-supplied cre | CWE-89 | [`GHSA-4px8-6x8g-722x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-4px8-6x8g-722x) · CVE-2026-52765 |
| `glpi-agent` | OS Command Injection via server-controlled archive filename in Deploy task | CWE-78 | [`GHSA-fh99-rgmp-c623`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-fh99-rgmp-c623) |
| `glpi-agent` | Deploy task Path Traversal in Tools::Archive | CWE-22/CWE-23 | [`GHSA-g2f7-8mp5-qw65`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-g2f7-8mp5-qw65) · CVE-2026-52768 |
| `glpi-agent` | glpi-agent ToolBox: Unauthenticated SNMP network scanning against arbitrary IP r | CWE-284/CWE-918 | [`GHSA-vv6x-8qfx-x756`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-vv6x-8qfx-x756) |
| `gogs` | Unbounded memory allocation in Git LFS batch API enables denial of service | CWE-400/CWE-770 | [`GHSA-m8mh-w9hx-mmjm`](https://github.com/gogs/gogs/security/advisories/GHSA-m8mh-w9hx-mmjm) |
| `gogs` | Image decompression bomb in avatar upload enables denial of service | CWE-400/CWE-409 | [`GHSA-v5vf-9g9p-p9fg`](https://github.com/gogs/gogs/security/advisories/GHSA-v5vf-9g9p-p9fg) |
| `gonic` | Incomplete fix of CVE-2026-49338: getCoverArt for playlists lacks the ownership  | CWE-639/CWE-862 | [`GHSA-364r-g89f-rmg3`](https://github.com/sentriz/gonic/security/advisories/GHSA-364r-g89f-rmg3) |
| `kirby` | Unauthenticated path traversal in Media::thumb — request filename not contained  | CWE-22 | [`GHSA-9vx2-j98c-p72w`](https://github.com/getkirby/kirby/security/advisories/GHSA-9vx2-j98c-p72w) |
| `monitoring-plugins` | SSRF and Redfish session-token disclosure via unvalidated @odata.id link in redf | CWE-20/CWE-918 | [`GHSA-96fx-pqc3-28xv`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-96fx-pqc3-28xv) |
| `openbabel` | NULL-pointer dereference in GAMESS-output MOPAC-charges block (gamessformat.cpp) | CWE-476 | [`GHSA-h28m-r6fh-m3vg`](https://github.com/openbabel/openbabel/security/advisories/GHSA-h28m-r6fh-m3vg) |
| `openbabel` | NULL-pointer dereference in Jaguar-output atomic-charge parser (jaguarformat.cpp | CWE-476 | [`GHSA-hx98-c7vh-jv7f`](https://github.com/openbabel/openbabel/security/advisories/GHSA-hx98-c7vh-jv7f) |
| `openbabel` | NULL-pointer dereference in Gaussian-output NMR-shift block (gaussformat.cpp) | CWE-476 | [`GHSA-jq53-w56h-97vp`](https://github.com/openbabel/openbabel/security/advisories/GHSA-jq53-w56h-97vp) |
| `openbabel` | NULL-pointer dereference in COF reader formalq handler (cofformat.cpp) | CWE-476 | [`GHSA-prrc-wr67-3q59`](https://github.com/openbabel/openbabel/security/advisories/GHSA-prrc-wr67-3q59) |
| `openbabel` | NULL-pointer/out-of-bounds dereference in WLN ring parser new_cycle (wln-nextmov | CWE-476 | [`GHSA-rfj6-35p6-w6gm`](https://github.com/openbabel/openbabel/security/advisories/GHSA-rfj6-35p6-w6gm) |
| `opendj` | OpenDJ JMX MBean-argument deserialization without a serial filter | CWE-502 | [`GHSA-qj63-3vrg-vcfx`](https://github.com/OpenIdentityPlatform/OpenDJ/security/advisories/GHSA-qj63-3vrg-vcfx) |
| `openstreetmap-website` | No server-side rate limit on unauthenticated Notes API (note/comment spam + emai | CWE-602/CWE-770 | [`GHSA-cx4c-mgj3-h7fc`](https://github.com/openstreetmap/openstreetmap-website/security/advisories/GHSA-cx4c-mgj3-h7fc) |
| `openstreetmap-website` | GPX trace archive decompression bomb causes memory-exhaustion DoS of the trace-i | CWE-400/CWE-409 | [`GHSA-g99w-vhvj-jqw4`](https://github.com/openstreetmap/openstreetmap-website/security/advisories/GHSA-g99w-vhvj-jqw4) |
| `Paymenter` | Coupon global max_uses bypass via concurrent checkout race (over-redemption) | CWE-362/CWE-367 | [`GHSA-4527-v9f7-43vr`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-4527-v9f7-43vr) |
| `Paymenter` | Credit-refund double-spend race condition in service downgrade (doUpgrade) | CWE-362 | [`GHSA-5gmm-hjfj-8ff7`](https://github.com/Paymenter/Paymenter/security/advisories/GHSA-5gmm-hjfj-8ff7) |
| `rancher` | Project resource-quota bypass via negative peer-namespace field.cattle.io/resour | CWE-770/CWE-863 | [`GHSA-gxxh-fqhr-87qc`](https://github.com/rancher/rancher/security/advisories/GHSA-gxxh-fqhr-87qc) |
| `statamic` | Missing authorization on navigation endpoint allows disclosure of restricted ent | CWE-639/CWE-862 | [`GHSA-qh8c-7588-qfrv`](https://github.com/statamic/cms/security/advisories/GHSA-qh8c-7588-qfrv) |
| `webpack-dev-server` | webpack-dev-server vulnerable to cross-site request forgery via internal develop | CWE-352/CWE-749 | [`GHSA-f5vj-f2hx-8m93`](https://github.com/webpack/webpack-dev-server/security/advisories/GHSA-f5vj-f2hx-8m93) · CVE-2026-14620 |

</details>

<details><summary>⚪ <b>Low</b> (12)</summary>

| Project | Vulnerability | CWE | Advisory |
|:--|:--|:--|:--|
| `glpi-agent` | Stored XSS via job tag field in ToolBox Inventory configuration (input/tag) | CWE-79 | [`GHSA-6995-8gmf-q4r2`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-6995-8gmf-q4r2) |
| `glpi-agent` | Stored XSS via SNMP community/authprotocol credential fields in ToolBox plugin | CWE-79 | [`GHSA-cwg9-jj5m-pq4q`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-cwg9-jj5m-pq4q) |
| `glpi-agent` | Stored XSS via inventory tag management in ToolBox plugin | CWE-79 | [`GHSA-m44h-67mc-8fxw`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-m44h-67mc-8fxw) |
| `glpi-agent` | Collect task compiles server-controlled regular expression without validation | CWE-1333 | [`GHSA-mgcf-xgv7-5w4x`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-mgcf-xgv7-5w4x) |
| `glpi-agent` | [Deploy] Improper Neutralization of Special Elements used in an OS Command ('OS  | CWE-78/CWE-345 | [`GHSA-r2hc-w524-5fwh`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-r2hc-w524-5fwh) |
| `glpi-agent` | Oracle inventory module uses unvalidated process username in shell su command | CWE-78 | [`GHSA-vwv6-85p7-mjvc`](https://github.com/glpi-project/glpi-agent/security/advisories/GHSA-vwv6-85p7-mjvc) |
| `kirby` | OptionsApi file:// SSRF / local file read via blueprint options.api.url | CWE-441/CWE-918 | [`GHSA-2m4q-xm8w-mpwf`](https://github.com/getkirby/kirby/security/advisories/GHSA-2m4q-xm8w-mpwf) |
| `monitoring-plugins` | logfile: legacy-DB migration follows attacker-planted symlink -> root file overw | CWE-59/CWE-377 | [`GHSA-w2gg-hx6w-24w3`](https://github.com/Linuxfabrik/monitoring-plugins/security/advisories/GHSA-w2gg-hx6w-24w3) |
| `NanaZip` | Unbounded memory allocation (DoS) in NanaZip UFS parser via unvalidated fs_bsize | CWE-400/CWE-789 | [`GHSA-m34h-jf84-m74h`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-m34h-jf84-m74h) · CVE-2026-55781 |
| `NanaZip` | Uncaught exception / unbounded allocation in NanaZip .NET single-file Extract()  | CWE-248/CWE-400 | [`GHSA-ppm9-5267-rq72`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-ppm9-5267-rq72) · CVE-2026-55780 |
| `NanaZip` | NULL pointer dereference in Extract() of all seven NanaZip custom archive handle | CWE-476 | [`GHSA-q67r-9cfh-xc29`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-q67r-9cfh-xc29) · CVE-2026-55783 |
| `NanaZip` | Unbounded memory allocation (DoS) in NanaZip WebAssembly parser via attacker-con | CWE-400/CWE-789 | [`GHSA-qxhc-2v6p-wm8m`](https://github.com/M2Team/NanaZip/security/advisories/GHSA-qxhc-2v6p-wm8m) · CVE-2026-55782 |

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

**Red Team / Offensive:** MCRTA · CRTS v2 · C3SA · Offensive Phishing Operations · RedInfraCraft · C2 Development
**Malware dev / exploitation:** Malware Development Essentials &amp; Intermediate · Advanced Process Injection v2 · OST2 **Exp4011** · **Fuzz1001** · **Dbg1011** · **Arch2821** · OffensiveRust · offensiveC#
**Cloud:** IAM · AWS AMI security · Azure Pentest Lab (SANS) · MCBTA
**Web / API / Mobile:** Hacking APIs · Practical Web AppSec · Mobile App Pentesting · PEH
**ICS / OT / IoT:** 210W-07/09 ICS · OT Security · Medical Device Security · IoT Pentesting
**AI security:** Claude Computer Use — From Prompt Injection to Raining Shells

<sub>→ full indexed set in <a href="https://github.com/Pig-Tail/Cert">Cert</a>.</sub>

---

<p align="center"><sub>Coordinated disclosure / collaboration → jorge@jmilla.es · <a href="https://twitter.com/jgonzalezmilla">@jgonzalezmilla</a></sub></p>
