## blow-tech

**Enterprise infrastructure doesn't break on my watch.**

Windows Server. Active Directory. Exchange Online. RHEL. VMware. These aren't
technologies I know — they're environments I've kept running.

Every script here was written because something broke, or nearly did.

---

## Repositories

### [powershell-admin-toolkit](https://github.com/blow-tech/powershell-admin-toolkit)
> Production automation for Windows Server and Microsoft 365.

AD lifecycle reporting. Exchange Online auditing. Environment health checks spanning
AD replication, DNS, certificates, disk, and services — output as a single HTML report.
Certificate expiry sweeps. Automated disk reclamation. Built from real incidents.
None of it is tutorial code.

`PowerShell 5.1+` `Active Directory` `Exchange Online` `Microsoft 365` `PKI / Certificates` `HTML Reports`

---

### [linux-admin-scripts](https://github.com/blow-tech/linux-admin-scripts)
> Bash tooling for RHEL server operations and auditing.

Health checks with threshold alerting. Rotated and compressed log parsing. Systemd
service monitoring with restart handling. Backup validation. Scheduled maintenance
and cleanup — structured for cron execution and consistent log output.

`Bash` `RHEL / CentOS` `systemd` `Log Parsing` `Monitoring` `Cron`

---

## Focus areas

| Domain | Skills |
|---|---|
| Windows Server | AD DS, DNS, DHCP, GPO, IIS, Certificate Authority, RSAT |
| Microsoft 365 | Exchange Online, Intune, SharePoint, Teams, Graph API |
| Scripting | PowerShell 5.1+, Bash, scheduled tasks, log parsing |
| Virtualisation | VMware ESXi / vCenter, VM lifecycle management |
| Linux | RHEL / CentOS, systemd, log rotation, auditing |
| Security & audit | Account lifecycle, lockout tracing, privileged access, mail flow |

---

## Active development

- `Get-EnvironmentHealthCheck.ps1` — unified AD, DNS, cert, disk, and service health with HTML report output
- `Security/` — privileged account audit, local admin enumeration, failed logon analysis
- `Intune/` — managed device reporting and compliance checks via Microsoft Graph API
- `Certificates/` — enterprise CA expiry sweep and renewal automation
- `linux-admin-scripts` — RHEL-specific checks and structured log output expansion

---

*Scripts built from production incidents. Enterprise AD and M365 environments.*
