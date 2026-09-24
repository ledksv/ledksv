# Ledion Mujaj

I got into cybersecurity from an unlikely place. I was working at a car wash when I came across a podcast with Ryan Montgomery randomly on Youtube. I had never thought about hacking before but the way he talked about it, breaking into systems legally, finding the weaknesses before the real attackers do, it stuck with me.

The notion of hacking into a system with permission, finding the flaws before someone with bad intentions does, that is what pulled me in.

I put the money I earned back into myself, worked through the CompTIA stack and started grinding labs and even built my very own AD home lab! I have not stopped since. Right now I am working toward HTB CPTS, CWES and CAPE.

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
| [labs](https://github.com/ledksv/lab-writeups) | Walkthroughs and pentest reports from labs I have completed |
| [skills](https://github.com/ledksv/red-team-skills) | Red team skills with links to demonstrated techniques |
| [oneliners](https://github.com/ledksv/pentest-oneliners) | Command cheatsheet for every phase |
| [Enum-recon](https://github.com/ledksv/Enum-recon) | Custom recon and enumeration script |

---

## Projects

### Vulnerability Assessment & Risk Prioritisation

Fingerprinted Mirth Connect 4.4.0 in [HTB Interpreter](https://github.com/ledksv/lab-writeups/blob/master/interpreter-htb.md), reproduced [CVE-2023-43208](https://github.com/ledksv/lab-writeups/blob/master/interpreter-htb.md) and traced exposed credentials and unsafe Python execution to root compromise. Reproduced SSRF ([CVE-2022-46364](https://github.com/ledksv/lab-writeups/blob/master/devarea-htb.md)) in [HTB DevArea](https://github.com/ledksv/lab-writeups/blob/master/devarea-htb.md), chaining a config file leak to expose administrator credentials. Assessed exploitability and security impact, documenting PoC evidence, CVSS scores and remediation recommendations.

`CVE Research` `Nmap` `Nikto` `CVSS` `Risk Assessment`

---

### Web Application & Infrastructure Security

Chained account takeover and RCE in [HTB Silentium](https://github.com/ledksv/lab-writeups/blob/master/silentium-htb.md) ([CVE-2025-58434](https://github.com/ledksv/lab-writeups/blob/master/silentium-htb.md), [CVE-2025-59528](https://github.com/ledksv/lab-writeups/blob/master/silentium-htb.md)), progressing through exposed container credentials and an internal Git service to root access. Exploited path traversal ([CVE-2025-49132](https://github.com/ledksv/lab-writeups/blob/master/pterodactyl-htb.md)) in [HTB Pterodactyl](https://github.com/ledksv/lab-writeups/blob/master/pterodactyl-htb.md) to extract database credentials and gain SSH access. Service discovery, VHost enumeration and web fuzzing across 30+ machines.

`Burp Suite` `ffuf` `Gobuster` `OWASP Top 10` `Web Exploitation`

---

### Active Directory Security

Built a self-hosted Windows Server 2022/2019 domain to simulate a real enterprise environment. Compromised from a low-privileged user to Domain Admin through Kerberoasting, Pass-the-Hash and DCSync. Used BloodHound and Impacket to investigate privilege escalation and authentication weaknesses.

`Active Directory` `BloodHound` `Kerberoasting` `DCSync` `Impacket`

---

### AI & LLM Application Security

Reproduced MCPJam Inspector RCE ([CVE-2026-23744](https://github.com/ledksv/lab-writeups/blob/master/kobold-htb.md)) in [HTB Kobold](https://github.com/ledksv/lab-writeups/blob/master/kobold-htb.md) and investigated Docker group privilege impact on container escape. Exploited a pre-auth WebSocket terminal bypass in [HTB DevHub](https://github.com/ledksv/lab-writeups/blob/master/devhub-htb.md)'s marimo notebook, bypassing authentication to gain code execution as a service user.

`LLM Security` `MCP` `OWASP LLM Top 10` `WebSocket` `AI Security`

---

### Security Automation & Tool Development

Built a [bash/Python recon script](https://github.com/ledksv/Enum-recon) that runs OSINT, DNS/SSL checks, Nmap and web enumeration from one command. Outputs everything into a structured folder with a Markdown report.

`Python` `Bash` `Automation` `Nmap NSE` `Reporting`

---

## Skills

Pentesting skills I have built through hands-on lab work, each linked to the writeup where I applied it:

- [Reconnaissance](https://github.com/ledksv/red-team-skills#reconnaissance) | service enumeration, VHost fuzzing, OSINT
- [Web Exploitation](https://github.com/ledksv/red-team-skills#web-exploitation) | SQLi, SSRF, file upload, path traversal
- [Active Directory](https://github.com/ledksv/red-team-skills#active-directory) | Kerberoasting, PTH, DCSync, AS-REP
- [Credential Access](https://github.com/ledksv/red-team-skills#credential-access) | hash cracking, brute forcing, credential harvesting
- [Privilege Escalation](https://github.com/ledksv/red-team-skills#privilege-escalation) | sudo abuse, container escape, library/PATH hijacking
