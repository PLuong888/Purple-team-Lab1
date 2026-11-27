# Evidence status and integrity notes

The screenshot checklist is a proposed collection target, not a requirement to fabricate every listed image. Missing images do not invalidate a well-written report if claims are appropriately qualified.

## Included evidence

| Phase | Filename | PDF page | Handling |
|---|---|---:|---|
| week01 | `day01-kali-boot-success.png` | 4 | Cropped from original PDF page |
| week01 | `day01-kali-snapshot.png` | 6 | Cropped from original PDF page |
| week01 | `day02-network-settings-kali.png` | 3 | Cropped from original PDF page |
| week01 | `day02-network-settings-metasploitable.png` | 2 | Cropped from original PDF page |
| week01 | `day02-metasploitable-ip-192.168.png` | 3 | Cropped from original PDF page |
| week01 | `day03-wazuh-install-success.png` | 8 | Cropped / credentials redacted |
| week01 | `day04-network-repair-dvwa.png` | 10 | Cropped from original PDF page |
| week01 | `day04-wazuh-authentication-failure-detected.png` | 11 | Cropped from original PDF page |
| week02 | `day08-hydra-kex-error.png` | 13 | Cropped from original PDF page |
| week02 | `day08-ssh-legacy-crypto-bypass-success.png` | 23 | Cropped / credentials redacted |
| week02 | `day09-sqli-or-1-equals-1.png` | 15 | Cropped from original PDF page |
| week02 | `day09-sqli-order-by-validation.png` | 17 | Cropped from original PDF page |
| week02 | `day09-sqli-union-database-version.png` | 18 | Cropped from original PDF page |
| week02 | `day09-sqlmap-database-enumeration.png` | 19 | Cropped from original PDF page |
| week02 | `day09-sqlmap-dump-users-cracked-passwords.png` | 30 | Cropped / credentials redacted |
| week02 | `day10-privilege-escalation-root-confirmed.png` | 33 | Cropped / credentials redacted |
| week02 | `day10-suid-binaries-nmap.png` | 34 | Cropped from original PDF page |
| week02 | `day11-msfconsole-search-vsftpd.png` | 35 | Cropped from original PDF page |
| week02 | `day11-meterpreter-vsftpd-root.png` | 36 | Cropped from original PDF page |
| week02 | `day11-meterpreter-getuid-root.png` | 37 | Cropped from original PDF page |
| week03 | `day13-wazuh-default-rules-review.png` | 38 | Cropped from original PDF page |
| week03 | `day13-local-rules-xml-content.png` | 39 | Cropped from original PDF page |
| week03 | `day13-rule-100002-in-dashboard.png` | 40 | Cropped from original PDF page |

## Important missing / unverified captures

### week01

- `day01-virtualbox-network-manager.png`
- `day01-passwd-change.png`
- `day02-isolation-confirmed.png (source PDF includes an earlier synthetic ping visual, not real isolation proof)`
- `day03-lvm-before.png`
- `day03-lvm-extend-command.png`
- `day03-lvm-after.png`
- `day04-vulnerability-detection-cve-list.png`

### week02

- `day07-nmap-sV-metasploitable2.png`
- `day07-wazuh-no-alert-nmap.png`
- `day09-wazuh-no-sqli-alert.png`
- `day10-wazuh-rule-5402-sudo.png (attribution unresolved)`

### week03

- `day13-wazuh-dashboard-mitre-attack-overview.png`
- `day13-custom-rule-100002-alert.png (custom rule firing unverified)`

## Consistency and publication checks

- **Synthetic ping image excluded:** The prior generated success screenshot cannot be used to support a 0%-packet-loss claim; preserve actual ping output if available.
- **Wazuh password:** The installation screenshot contained an exposed admin password; the relevant line has been redacted from the public crop. Rotate the original password because it was already shown in the source file.
- **Privileged output:** The root-confirmation screenshot is cropped before `/etc/shadow` data.
- **sqlmap credentials:** Plaintext demo passwords and hashes are obscured in the screenshot; the report retains only the learning outcome.
- **Custom rule:** A rule listed in Wazuh is not the same as a triggered alert.
- **Privilege-escalation detection:** No original rule-5402 event is attributable to Metasploitable2; mark unverified.
- **Nightly timestamps and metadata:** Source screenshots sometimes show different dates and adapters during troubleshooting; interpret them as stages of work, not a single consistent snapshot.
- **No source PDF or unredacted page copies** are included in this package, because those may leak sensitive material.

## Advice for portfolio reviewers

Open `README.md` first, then choose any `docs/*.docx` report. Each Word report includes the most relevant images inline. Full-size sanitized copies are filed by week in `screenshots/`.
