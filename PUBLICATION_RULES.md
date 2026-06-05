# DrPlaga.sh - Publication Rules

This document defines the minimum rules before publishing code, writeups, payload analysis, CVE notes or security research under the `drplagash` GitHub profile.

The goal is simple: publish useful defensive material without leaking sensitive data, enabling abuse or creating unnecessary risk.

---

## Core rule

Do not publish anything that is unclear, untested, unsafe or not properly documented.

If something is old, messy or potentially sensitive, keep it private until reviewed.

---

## Before publishing

Every file, script, writeup or report must be checked for:

```text
Secrets:
- API keys
- Tokens
- Passwords
- Cookies
- Session IDs
- Private SSH keys
- Private certificates
- Cloud credentials
```

```text
Sensitive data:
- Real credentials
- Dumps
- Leaks
- Personal data
- Internal hostnames
- Private infrastructure details
- Non-public IP mappings
- Customer/client data
```

```text
Operational risk:
- Destructive commands
- Hardcoded targets
- Persistence
- Evasion
- Credential theft
- Malware-like behavior
- Third-party targeting
```

---

## Public repository rules

Allowed:

* CTF writeups.
* DockerLabs notes.
* Lab-only CVE analysis.
* Defensive PoCs.
* Sanitized payload analysis.
* Detection rules.
* Bash/Python utilities.
* Recon scripts for authorized environments.
* Documentation and methodology.

Not allowed:

* Live malware binaries.
* Weaponized payloads.
* Real stolen credentials.
* Dumps or leaked data.
* Third-party exploitation guides.
* Persistence or evasion tooling.
* Scripts with hardcoded victims.
* Anything that enables abuse without defensive context.

---

## Required documentation

Every public script or tool should include:

```text
Purpose:
Scope:
Requirements:
Usage:
Output:
Safety notes:
Known limitations:
```

Every CTF writeup should include:

```text
Platform:
Scope:
Enumeration:
Exploitation:
Privilege escalation:
Evidence:
Defensive notes:
Lessons learned:
```

Every CVE analysis should include:

```text
CVE ID:
Affected product:
Lab scope:
Impact:
Reproduction:
Detection:
Mitigation:
References:
Disclaimer:
```

Every payload analysis should include:

```text
Source:
Sanitized payload:
Decoding steps:
Behavior:
Indicators:
Detection:
Mitigation:
Confidence:
Conclusion:
```

---

## Sanitization checklist

Before committing:

* [ ] No API keys.
* [ ] No tokens.
* [ ] No passwords.
* [ ] No cookies.
* [ ] No private keys.
* [ ] No real credentials.
* [ ] No dumps.
* [ ] No sensitive screenshots.
* [ ] No private infrastructure details.
* [ ] No unintended target IPs.
* [ ] No local absolute paths with usernames.
* [ ] No `.env` files.
* [ ] No backup files with secrets.
* [ ] No raw malware binaries.
* [ ] No exploit instructions against third-party systems.

---

## Code quality checklist

Before publishing code:

* [ ] The script runs.
* [ ] The script has a clear name.
* [ ] The script has usage instructions.
* [ ] Dangerous actions are not default.
* [ ] Inputs are validated.
* [ ] Errors are handled.
* [ ] Outputs are documented.
* [ ] Dependencies are listed.
* [ ] No secrets are hardcoded.
* [ ] The README explains the purpose and scope.

---

## Commit message style

Use short and clear messages.

Good examples:

```text
Add DockerLabs writeup template
Update payload analysis README
Add Nmap parser script
Fix recon output validation
Add CVE lab notes
```

Bad examples:

```text
update
stuff
final
fix
asdasd
probando
```

Sí, `asdasd` funciona. También funciona comer sopa con un tenedor. No por eso hay que hacerlo.

---

## Repository placement

Use the correct repository:

```text
ctf-writeups       -> CTFs, DockerLabs, PortSwigger, VulnHub, HTB, THM
cve-lab-pocs       -> CVE analysis and lab-only PoCs
security-tools     -> scripts, parsers, automation, recon helpers
payload-analysis   -> payload decoding, IOCs, YARA/Sigma/Suricata, reports
drplagash          -> profile README and repository map only
CodeBugBox         -> old private backup, not public
```

---

## Migration from private repo

When moving old material from `CodeBugBox`:

```text
1. Review.
2. Test.
3. Sanitize.
4. Improve.
5. Document.
6. Add disclaimer.
7. Move to the correct public repo.
8. Commit with a clear message.
```

Do not bulk-migrate old code.

Old code should be treated as untrusted until reviewed.

---

## Disclaimer template

Use this disclaimer when needed:

```text
This material is provided for educational, defensive and authorized lab use only.
Do not use it against third-party systems.
Do not use it for unauthorized access, disruption, persistence, evasion or credential theft.
```

---

## Operating principle

Evidence before noise.

Defensive use only.

Authorized labs only.

**Menos humo, más evidencia.**
