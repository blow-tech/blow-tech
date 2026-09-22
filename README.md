# blow-tech

### Infrastructure Engineering • Systems Administration • Automation • Monitoring

Infrastructure engineer working across Windows Server, Linux, Microsoft 365,
VMware, infrastructure as code, configuration management, and observability.

The projects here focus on practical infrastructure engineering: automating
repeatable operations, standardizing deployments, improving monitoring and
auditability, and managing infrastructure through version-controlled code.

> Public repositories are sanitized and contain no production credentials,
> customer information, or environment-specific secrets.

---

## Featured Infrastructure Projects

### [labhandzone-infra](https://github.com/blow-tech/labhandzone-infra)
> Infrastructure-as-code lab combining Terraform, VMware vSphere, Active Directory,
> SQL Server, WSUS, file services, and Ansible automation.

Terraform provisions virtual infrastructure on vSphere while Ansible handles
Windows configuration and service deployment.

The environment includes:

- Active Directory forest deployment
- Windows Server virtual machines
- SQL Server nodes
- iSCSI-backed storage
- File services
- WSUS
- GPO-driven patching
- PowerShell-based configuration
- Automated validation through GitHub Actions

CI checks include Terraform formatting and validation, Ansible syntax validation,
YAML linting, and rendered PowerShell template syntax checks.

`Terraform` `VMware vSphere` `Ansible` `Windows Server` `Active Directory`
`SQL Server` `WSUS` `PowerShell` `GitHub Actions`

---

### [fleet-monitoring-stack](https://github.com/blow-tech/fleet-monitoring-stack)
> Automated monitoring platform for Linux fleets using Prometheus, Grafana,
> Alertmanager, Ansible, Docker, and Kubernetes.

Provides centralized monitoring for RHEL-based systems with Prometheus target
management driven from Ansible inventory.

Supports two deployment models:

- VM-based deployment using Ansible and Docker Compose
- Kubernetes deployment using Argo CD GitOps with Istio service mesh

The goal is to keep monitoring configuration aligned with infrastructure changes
without requiring manual edits to Prometheus target configuration.

`Prometheus` `Grafana` `Alertmanager` `Ansible` `Docker Compose`
`Kubernetes` `Argo CD` `Istio` `GitOps` `RHEL` `GitHub Actions`

---

## Automation & Operations Projects

### [powershell-admin-toolkit](https://github.com/blow-tech/powershell-admin-toolkit)
> Operational automation for Windows Server and Microsoft 365 administration.

Includes tooling for:

- Active Directory lifecycle reporting
- Exchange Online auditing
- Microsoft 365 administration
- Password-expiry notifications
- Privileged-role auditing
- Disk reclamation
- Infrastructure health reporting
- AD replication checks
- DNS validation
- Certificate monitoring
- Storage and service health checks

Health information is consolidated into HTML reports for operational review.

`PowerShell 5.1+` `Active Directory` `Exchange Online` `Microsoft 365`
`Microsoft Graph` `Windows Server` `HTML Reporting`

---

### [linux-audit-toolkit](https://github.com/blow-tech/linux-audit-toolkit)
> Read-only Linux audit framework for RHEL-based environments with fleet-wide
> deployment through Ansible.

Includes focused audit tooling for:

- Disk and inode utilization
- Login/logout activity
- Brute-force indicators
- File and directory permission drift
- Service health
- CPU, memory, and swap utilization
- Local accounts and sudo configuration
- Cron jobs and systemd timers
- Listening ports and firewall state
- Web server log analysis
- Rotated and compressed `.gz` log processing

An orchestration layer consolidates results into timestamped reports with
consistent exit codes suitable for scheduled execution and monitoring integration.

An idempotent Ansible role supports fleet-wide deployment using systemd timers
or cron.

`Bash` `RHEL / CentOS` `Ansible` `systemd` `Security Auditing`
`Monitoring` `Log Analysis`

---

### [linux-admin-scripts](https://github.com/blow-tech/linux-admin-scripts)
> Operational Bash tooling for Linux administration and maintenance.

Includes:

- Health checks with threshold-based alerting
- Rotated and compressed log parsing
- systemd service monitoring
- Controlled restart handling
- Backup validation
- Scheduled maintenance
- Cleanup automation
- Consistent logging and exit codes

Designed for both interactive administration and unattended scheduled execution.

`Bash` `RHEL / CentOS` `systemd` `Log Analysis` `Monitoring` `Cron`

---

## Technical Focus

| Domain | Technologies |
|---|---|
| Windows Infrastructure | Windows Server, AD DS, DNS, DHCP, GPO, IIS, AD CS, RSAT |
| Microsoft 365 | Exchange Online, Intune, SharePoint, Teams, Entra ID, Microsoft Graph |
| Azure | Virtual Machines, VNets, Storage, Entra ID, Azure Monitor, RBAC, Az PowerShell |
| Virtualization | VMware ESXi, vCenter, VM provisioning, lifecycle management |
| Infrastructure as Code | Terraform, reusable modules, declarative infrastructure |
| Configuration Management | Ansible, roles, inventories, Jinja2 templates |
| Linux | RHEL / CentOS, Bash, systemd, SELinux, logrotate |
| Containers | Docker, Docker Compose |
| Kubernetes | Kubernetes, Argo CD, GitOps, Istio |
| Monitoring | Prometheus, Grafana, Alertmanager, health checks, log analysis |
| CI/CD | GitHub Actions, linting, syntax validation, Terraform validation |
| Automation | PowerShell, Bash, Ansible, scheduled tasks, cron |
| Security & Audit | PIM, sudoers, account lifecycle, permission auditing, lockout tracing |

---

## Engineering Approach

### Root-cause focused

Troubleshooting starts with understanding why a failure occurred rather than only
addressing the immediate symptom.

### Automation where it adds value

Repeated operational tasks are converted into reusable tooling with predictable
inputs, outputs, logging, and failure handling.

### Safe by default

Audit and reporting tools are designed to be read-only unless a change is explicitly
required. Infrastructure changes should be visible, intentional, and repeatable.

### Designed for scale

Solutions should work for one system without preventing their use across larger
environments through Ansible, PowerShell remoting, scheduled execution, or
centralized orchestration.

### Infrastructure as code

Where practical, infrastructure and configuration are represented as
version-controlled code so environments can be reviewed, reproduced, validated,
and improved over time.

### Validation before deployment

Projects use automated checks where appropriate, including formatting validation,
syntax checks, linting, configuration validation, and CI workflows.

---

## Current Areas of Interest

Currently expanding work around:

- Infrastructure as code
- Automated Windows Server deployment
- VMware provisioning
- Configuration management
- Linux fleet management
- Prometheus/Grafana observability
- Kubernetes
- GitOps with Argo CD
- CI validation
- Hybrid Windows/Linux infrastructure automation

---

## Repository Standards

Projects generally aim to include:

- Clear documentation
- Reusable configuration
- Consistent logging
- Predictable exit codes
- Idempotent automation where applicable
- CI validation
- Separation of configuration from code
- No credentials or secrets committed to source control
- Safe defaults for audit and reporting operations

---

## Technology Overview

`PowerShell` `Bash` `Python` `Terraform` `Ansible` `Jinja2`

`Windows Server` `Active Directory` `Microsoft 365` `Azure`

`RHEL` `Linux` `VMware vSphere`

`Docker` `Kubernetes` `Argo CD` `Istio`

`Prometheus` `Grafana` `Alertmanager`

`Git` `GitHub Actions`
