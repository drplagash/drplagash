# Contributing

Thanks for your interest in contributing to DrPlaga.sh repositories.

This GitHub profile is focused on cybersecurity learning, defensive research, CTF practice, lab-based CVE analysis, payload analysis and security tooling.

Contributions are welcome when they improve clarity, documentation, defensive value or code quality.

---

## General rules

Contributions must follow these principles:

* Defensive use only
* Authorized environments only
* No third-party targeting
* No credential theft
* No persistence or evasion tooling
* No malware deployment
* No live malware binaries
* No stolen data, dumps or leaks
* No secrets, tokens, API keys or credentials
* No unsafe publication of weaponized payloads

---

## Accepted contributions

Good contributions include:

* Documentation improvements
* Typo fixes
* Safer examples
* Better usage instructions
* Defensive detection logic
* Lab-only improvements
* Script error handling
* Input validation
* Output formatting
* References to official advisories or trusted sources
* Sanitized payload analysis improvements

---

## Not accepted

The following contributions will not be accepted:

* Code targeting real third-party systems
* Weaponized exploit chains
* Credential theft logic
* Persistence mechanisms
* Evasion techniques
* Stealth tooling
* Live malware samples
* Dumps or leaked data
* Hardcoded victims
* Hardcoded secrets
* Unclear PoCs without defensive context
* Pull requests with unexplained code

---

## Repository placement

Use the correct repository:

```text
ctf-writeups       -> CTFs, DockerLabs, PortSwigger, VulnHub, HTB, THM
cve-lab-pocs       -> CVE analysis and lab-only PoCs
security-tools     -> scripts, parsers, automation, recon helpers
payload-analysis   -> payload decoding, IOCs, YARA/Sigma/Suricata, reports
drplagash          -> profile README, repository map and project policy files
```

---

## Pull request checklist

Before opening a pull request:

* [ ] The contribution has a clear purpose.
* [ ] The code or document belongs in the selected repository.
* [ ] No secrets are included.
* [ ] No sensitive data is included.
* [ ] No live malware is included.
* [ ] No third-party targeting is included.
* [ ] Usage is documented.
* [ ] Limitations are documented.
* [ ] Defensive value is clear.
* [ ] References are included when needed.

---

## Code expectations

For scripts and tools:

* Use clear names.
* Validate inputs.
* Handle errors.
* Avoid destructive defaults.
* Do not hardcode targets.
* Do not hardcode credentials.
* Document dependencies.
* Include usage examples.
* Include expected output.

---

## Writeup expectations

For CTF or lab writeups:

* Explain scope.
* Include enumeration.
* Include exploitation path.
* Include privilege escalation path if applicable.
* Redact flags if needed.
* Avoid real credentials.
* Add defensive notes when possible.
* Add lessons learned.

---

## CVE analysis expectations

For CVE-related material:

* Include CVE ID.
* Include affected product/version.
* Include lab scope.
* Include impact.
* Include safe reproduction notes.
* Include detection ideas.
* Include mitigation.
* Include references.

Avoid publishing exploit code without context, mitigation or a controlled lab explanation.

---

## Payload analysis expectations

For payload analysis:

* Use sanitized payloads.
* Document decoding steps.
* Extract indicators.
* Explain behavior.
* Include detection ideas.
* Include confidence level.
* Do not publish live malware or weaponized payloads.

---

## Commit messages

Use clear commit messages.

Good examples:

```text
Add DockerLabs writeup template
Improve payload analysis checklist
Fix Nmap output parser
Add CVE mitigation notes
Update repository map
```

Bad examples:

```text
update
fix
stuff
final
test
asdasd
```

Sí, `asdasd` compila como mensaje de commit, pero también una piedra sirve de mouse si estás suficientemente desesperado.

---

## Disclaimer

All contributions must support educational, defensive and authorized lab use only.

Do not contribute material intended for unauthorized access, disruption, credential theft, persistence, evasion or abuse.

**Menos humo, más evidencia.**
