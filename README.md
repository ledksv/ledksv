# Ledion Mujaj

I wasn't always in tech. I was working at a car wash when I came across a documentary featuring Ryan Montgomery — a hacker who exposes predators and talks openly about what offensive security actually looks like. That was it for me. I went deep into researching the field, and the idea of breaking into systems with permission — getting there before the real attackers do, so defenders know exactly what they're up against — completely hooked me.

I reinvested in myself, worked through CompTIA certifications, and started grinding HackTheBox. The more I learned, the more I wanted to go deeper. Right now I'm working toward HTB CPTS, CWES, and CAPE.

Everything I learn gets documented here and on [l3dsec.com](https://l3dsec.com).

---

## Certifications

| Certification | Date | Status |
|---------------|------|--------|
| HTB CPTS | Est. Dec 2026 | In Progress |
| HTB CWES | Est. 2027 | In Progress |
| HTB CAPE | Est. 2027 | In Progress |
| CompTIA Cloud+ | May 2025 | Achieved |
| ITIL Foundation | May 2025 | Achieved |
| CompTIA Network+ (N10-008) | Dec 2024 | Achieved |
| CompTIA A+ Core 1 (220-1101) | Oct 2024 | Achieved |
| CompTIA A+ Core 2 (220-1102) | Dec 2024 | Achieved |
| CompTIA ITF+ (FC0-U61) | Aug 2024 | Achieved |

---

## Navigation

| Section | Description |
|---------|-------------|
| [labs/](labs/README.md) | HTB and VulnHub walkthroughs |
| [reports/](reports/README.md) | Penetration test reports |
| [skills/](skills/README.md) | Red team skills with links to demonstrated techniques |
| [oneliners/](oneliners/README.md) | Command cheatsheet for every phase |
| [projects/](projects/README.md) | Research projects and tooling |
| [tools/](tools/README.md) | Custom scripts and tools |

---

## Projects

### Vulnerability Assessment & Risk Prioritisation

Fingerprinted Mirth Connect 4.4.0 in HTB Interpreter, reproduced CVE-2023-43208 and traced exposed credentials and unsafe Python execution to root compromise. Reproduced SSRF (CVE-2022-46364) in HTB DevArea, chaining a config file leak to expose administrator credentials. Assessed exploitability and security impact, documenting PoC evidence, CVSS scores and remediation recommendations.

`CVE Research` `Nmap` `Nikto` `CVSS` `Risk Assessment`

---

### Web Application & Infrastructure Security

Chained account takeover and RCE in HTB Silentium (CVE-2025-58434, CVE-2025-59528), progressing through exposed container credentials and an internal Git service to root access. Exploited path traversal (CVE-2025-49132) in HTB Pterodactyl to extract database credentials and gain SSH access. Service discovery, VHost enumeration and web fuzzing across 30+ machines.

`Burp Suite` `ffuf` `Gobuster` `OWASP Top 10` `Web Exploitation`

---

### Active Directory Security

Built a self-hosted Windows Server 2022/2019 domain to simulate a real enterprise environment. Compromised from a low-privileged user to Domain Admin through Kerberoasting, Pass-the-Hash and DCSync. Used BloodHound and Impacket to investigate privilege escalation and authentication weaknesses.

`Active Directory` `BloodHound` `Kerberoasting` `DCSync` `Impacket`

---

### AI & LLM Application Security

Reproduced MCPJam Inspector RCE (CVE-2026-23744) in HTB Kobold and investigated Docker group privilege impact on container escape. Exploited a pre-auth WebSocket terminal bypass in HTB DevHub's marimo notebook, bypassing authentication to gain code execution as a service user.

`LLM Security` `MCP` `OWASP LLM Top 10` `WebSocket` `AI Security`

---

### Security Automation & Tool Development

Developed a [bash/Python reconnaissance pipeline](https://github.com/ledksv/Enum-recon) integrating OSINT, DNS/SSL checks, Nmap and web enumeration, cutting manual enumeration time significantly. Automated vulnerability scanning and SMB/SNMP enumeration with structured Markdown report output.

`Python` `Bash` `Automation` `Nmap NSE` `Reporting`

---

## Labs

30+ walkthroughs across HackTheBox and VulnHub. See [labs/README.md](labs/README.md) for the full list.

---

## Skills

Five red team skill areas, each with links to where the technique was demonstrated:

- [Reconnaissance](skills/README.md#reconnaissance) — service enumeration, VHost fuzzing, OSINT
- [Web Exploitation](skills/README.md#web-exploitation) — SQLi, SSRF, file upload, path traversal
- [Active Directory](skills/README.md#active-directory) — Kerberoasting, PTH, DCSync, AS-REP
- [Credential Access](skills/README.md#credential-access) — hash cracking, brute forcing, credential harvesting
- [Privilege Escalation](skills/README.md#privilege-escalation) — sudo abuse, container escape, library/PATH hijacking
