# DrPlaga.sh - Repository Map

This document defines the purpose of each public repository under the `drplagash` GitHub profile.

The goal is to keep the project organized, readable and useful for cybersecurity learning, defensive research, CTF practice and tooling.

---

## Public repositories

```text
drplagash/
├── drplagash/          # Public GitHub profile
├── ctf-writeups/       # CTFs, DockerLabs and vulnerable machines
├── cve-lab-pocs/       # CVE analysis and lab-only PoCs
├── security-tools/     # Personal scripts and defensive utilities
├── payload-analysis/   # Defensive payload analysis and detection notes
└── CodeBugBox/         # Old private backup repository
```

---

## `drplagash`

Purpose:

* Public GitHub profile.
* Professional presentation.
* Project overview.
* Main links.
* Repository index.

This repository should stay clean and minimal.

Content:

```text
README.md
REPOS_MAP.md
```

Do not use this repository for scripts, PoCs, payloads or writeups.

---

## `ctf-writeups`

Purpose:

* CTF writeups.
* DockerLabs machines.
* PortSwigger labs.
* VulnHub machines.
* TryHackMe rooms.
* Hack The Box machines.
* Local vulnerable labs.

Current structure:

```text
ctf-writeups/
├── dockerlabs/
├── portswigger/
├── vulnhub/
├── tryhackme/
├── hackthebox/
├── local-labs/
└── templates/
```

What belongs here:

* Machine walkthroughs.
* Enumeration notes.
* Nmap results.
* Gobuster/FFUF results.
* Exploitation path.
* Privilege escalation notes.
* Screenshots.
* Defensive lessons.

What does not belong here:

* Real targets.
* Real credentials.
* Tokens.
* Dumps.
* Malware.
* Unrelated scripts.

---

## `cve-lab-pocs`

Purpose:

* CVE analysis in controlled environments.
* Proof-of-concept code tested only in labs.
* Reproduction notes.
* Detection logic.
* Mitigation notes.

Expected structure:

```text
cve-lab-pocs/
├── CVE-YYYY-NNNN-product-name/
│   ├── README.md
│   ├── lab/
│   ├── exploit/
│   ├── detection/
│   ├── mitigation/
│   ├── screenshots/
│   └── notes.md
├── docs/
├── examples/
└── templates/
```

What belongs here:

* CVE summaries.
* Lab setup.
* Safe PoCs.
* Detection rules.
* Mitigation notes.
* Vendor references.
* NVD/CISA/vendor links.

What does not belong here:

* Uncontrolled exploit code.
* Third-party target instructions.
* Credential theft.
* Persistence/evasion tooling.
* Live malware.
* Exploits without context.

---

## `security-tools`

Purpose:

* Personal scripts.
* Defensive utilities.
* Recon helpers.
* Parsers.
* Automation.
* CTI helpers.
* Linux/network tools.

Current structure:

```text
security-tools/
├── recon/
├── web/
├── parsing/
├── automation/
├── linux/
├── network/
├── cti/
├── templates/
└── docs/
```

What belongs here:

* Bash scripts.
* Python scripts.
* Recon wrappers.
* Nmap helpers.
* Log parsers.
* IOC parsers.
* Report generators.
* Automation scripts.

What does not belong here:

* Full CTF writeups.
* CVE PoCs.
* Raw payload analysis.
* Hardcoded secrets.
* Destructive scripts without warnings.
* Offensive tooling without defensive context.

---

## `payload-analysis`

Purpose:

* Defensive analysis of suspicious payloads.
* Decoding notes.
* Sanitized samples.
* IOCs.
* Detection logic.
* T-Pot/honeypot payload review.
* CTF/lab payload documentation.

Expected structure:

```text
payload-analysis/
├── templates/
├── tpot/
├── web/
├── malware-like/
├── encoded/
├── yara/
├── sigma/
├── suricata/
├── scripts/
├── reports/
└── sanitized-samples/
```

What belongs here:

* Sanitized payloads.
* Decoded payloads.
* HTTP attack payload notes.
* Command injection payloads.
* SQLi/XSS/LFI/RFI payload analysis.
* YARA rules.
* Sigma rules.
* Suricata rules.
* IOC extraction.
* Honeypot observations.

What does not belong here:

* Live malware binaries.
* Weaponized payloads.
* Real credentials.
* Tokens.
* Dumps.
* Private infrastructure details.
* Third-party targeting instructions.

---

## Private repository

## `CodeBugBox`

Purpose:

* Old private backup.
* Historical code.
* Unreviewed scripts.
* Material pending cleanup.

Migration rule:

Do not move everything at once.

Process:

```text
1. Review old code.
2. Test locally.
3. Remove secrets and sensitive data.
4. Improve structure.
5. Add README.
6. Add disclaimer if needed.
7. Move to the correct public repository.
```

---

## Future repositories

Possible future repos:

```text
crypto-labs
hardware-hacking-lab
```

Only create them when there is enough clean content to justify separate repositories.

Until then:

* Crypto notes can stay private or documented locally.
* Hardware hacking notes can stay private until sanitized.

---

## Publishing rules

Before publishing anything:

* No credentials.
* No tokens.
* No API keys.
* No cookies.
* No dumps.
* No sensitive files.
* No private IPs unless intentionally included for lab context.
* No real victim data.
* No live malware.
* No third-party targeting.
* No unclear PoCs.

Every public item should include:

* Purpose.
* Scope.
* Requirements.
* Usage.
* Output.
* Safety notes.
* References when needed.

---

## Operating principle

Evidence before noise.

Defensive use only.

Authorized labs only.

**Menos humo, más evidencia.**
