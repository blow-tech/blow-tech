# blow-tech

**Infrastructure Engineer | Windows • Linux • Microsoft 365 • VMware • Automation**

7+ years running hybrid Windows, Linux and Microsoft 365 environments. I build
automation that is repeatable, auditable and safe to run: read-only by default,
validated in CI, and designed around restore and rollback first.

> All public repositories are sanitized: no production credentials,
> customer data or environment-specific secrets.

---

## Featured projects

### [labhandzone-infra](https://github.com/blow-tech/labhandzone-infra)
Terraform and Ansible lab on vSphere: AD forest, SQL Server Failover Cluster
Instance on iSCSI, file services, and WSUS with GPO-driven patch rings.
CI runs Terraform fmt/validate, Ansible syntax checks, YAML linting and
PowerShell template validation.

`Terraform` `vSphere` `Ansible` `Active Directory` `SQL Server` `GitHub Actions`

### [VMware-to-Hyper-migration](https://github.com/blow-tech/VMware-to-Hyper-migration)
Phase-gated methodology for migrating VMware to Hyper-V / Azure Stack HCI.
Each phase produces evidence (a filled CSV, a passed checklist, a proven
restore) before the next one starts. Domain controllers are rebuilt on the
target platform, never P2V'd, to avoid USN rollback and SYSVOL risk.

`Ansible` `PowerCLI` `Hyper-V` `Azure Stack HCI` `Storage Spaces Direct`

### [fleet-monitoring-stack](https://github.com/blow-tech/fleet-monitoring-stack)
Prometheus, Grafana and Alertmanager for RHEL fleets, with scrape targets
generated from Ansible inventory so monitoring follows infrastructure changes.
Deployable as VMs (Docker Compose) or on Kubernetes (Argo CD, Istio).

`Prometheus` `Grafana` `Ansible` `Kubernetes` `Argo CD`

### [linux-audit-toolkit](https://github.com/blow-tech/linux-audit-toolkit)
Read-only audit framework for RHEL: disk, accounts and sudo, permission drift,
listening ports, brute-force indicators and rotated `.gz` log analysis.
Consistent exit codes for scheduled runs, deployed fleet-wide through an
idempotent Ansible role.

`Bash` `RHEL` `Ansible` `systemd`

### [powershell-admin-toolkit](https://github.com/blow-tech/powershell-admin-toolkit)
Operational automation for Windows Server and Microsoft 365: AD lifecycle
reporting, Exchange Online auditing, privileged-role auditing, password-expiry
notifications, health reporting, and a read-only M365 reporting kit (Graph,
Exchange and Entra sign-in exports).

`PowerShell` `Active Directory` `Exchange Online` `Microsoft Graph`

---

## Core skills

| Area | Technologies |
|---|---|
| Windows & identity | Windows Server, Active Directory, DNS, DHCP, GPO, AD CS |
| Microsoft 365 & Azure | Exchange Online, Entra ID, Intune, Microsoft Graph, Az PowerShell |
| Virtualization | VMware vSphere, Hyper-V, Azure Stack HCI |
| Linux | RHEL, Bash, systemd, SELinux, logrotate |
| IaC & configuration | Terraform, Ansible |
| Monitoring & CI | Prometheus, Grafana, Alertmanager, GitHub Actions |
