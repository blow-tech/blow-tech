# blow-tech

Systems administrator / infrastructure engineer working across Windows Server,
Active Directory, Exchange Online, Microsoft 365, RHEL, and VMware. The
scripts and tooling here come out of production environments built to fix
recurring operational problems and reduce manual work, not to demonstrate
syntax.

---

## Repositories

### [powershell-admin-toolkit](https://github.com/blow-tech/powershell-admin-toolkit)
> Production automation for Windows Server and Microsoft 365.

AD lifecycle reporting, Exchange Online auditing, and environment health
checks spanning AD replication, DNS, certificates, disk, and core services
consolidated into a single HTML report. Includes automated disk reclamation,
password-expiry notifications, and PIM role auditing.

`PowerShell 5.1+` `Active Directory` `Exchange Online` `Microsoft 365` `Graph API` `HTML Reports`

---

### [linux-audit-toolkit](https://github.com/blow-tech/linux-audit-toolkit)
> Read-only production audit suite for RHEL servers, with Ansible for fleet-wide rollout.

Ten focused Bash scripts covering disk/inode usage, login/logout and
brute-force detection, file & directory permission drift, service health
(httpd/nginx/tomcat + core daemons), web server log analysis across rotated
`.gz` archives, CPU/RAM/swap, user account & sudoers auditing, cron/systemd
timers, and listening ports/firewall state plus an orchestrator that
consolidates everything into one timestamped report with standard exit codes
for monitoring integration. Ships with an idempotent Ansible role for
deploying and scheduling across an entire fleet via systemd timers or cron.

`Bash` `RHEL / CentOS` `Ansible` `systemd` `Security Auditing` `Monitoring`

---

### [linux-admin-scripts](https://github.com/blow-tech/linux-admin-scripts)
> Bash tooling for RHEL server operations and maintenance.

Health checks with threshold alerting, rotated/compressed log parsing,
systemd service monitoring with restart handling, backup validation, and
scheduled maintenance/cleanup structured for cron execution with
consistent log output.

`Bash` `RHEL / CentOS` `systemd` `Log Parsing` `Monitoring` `Cron`

---

## Focus areas

| Domain | Skills |
|---|---|
| Windows Server | AD DS, DNS, DHCP, GPO, IIS, Certificate Authority (ADCS), RSAT |
| Microsoft 365 | Exchange Online, Intune, SharePoint, Teams, Entra ID, Graph API |
| Cloud | Azure (VMs, VNets, Storage, Entra ID, Monitor, RBAC) Az PowerShell |
| Virtualization | VMware ESXi / vCenter, VM provisioning and lifecycle management |
| Linux | RHEL / CentOS, systemd, SELinux, log rotation, production auditing |
| Automation | PowerShell, Bash, Ansible (playbooks/roles), scheduled tasks |
| Security & audit | Account lifecycle, privileged access (PIM/sudoers), lockout tracing, mail flow |

## How I work

- **Root-cause first.** Fixes address why something broke, not just the
  symptom in front of me.
- **Production-safe by default.** Audit and reporting tooling here is
  read-only unless explicitly stated no surprise restarts or config drift.
- **Built to scale past one server.** Scripts are designed to run standalone
  *or* roll out fleet-wide via Ansible, so a fix for one host becomes a
  standard for all of them.

---
