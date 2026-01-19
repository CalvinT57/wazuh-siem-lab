# Wazuh SIEM Deployment and Endpoint Monitoring (Ubuntu + Windows 11)

## Overview
This project documents a hands-on deployment of the Wazuh SIEM stack on Ubuntu 24.04.3 LTS, including manager, indexer, and dashboard components. A Windows 11 endpoint agent was enrolled and monitoring was validated by generating and analyzing security alerts in the Wazuh dashboard.

## Objectives
- Deploy and validate core Wazuh services (manager, indexer, dashboard)
- Confirm system readiness (OS/network/disk validation)
- Enroll a Windows 11 endpoint agent
- Verify log ingestion and alert generation
- Review alert metadata and rule details for investigation

## Lab Environment
- Host platform: VMware Fusion (virtualized lab)
- SIEM server OS: Ubuntu 24.04.3 LTS
- Endpoint OS: Windows 11
- Tools/Components: Wazuh manager, Wazuh indexer, Wazuh dashboard, Wazuh agent

## Methodology (High Level)
1. Validated Ubuntu OS version, IP configuration, and storage capacity
2. Installed Wazuh stack and verified services were running
3. Accessed Wazuh dashboard and confirmed availability
4. Deployed and enrolled a Windows 11 agent
5. Validated alert generation and performed alert review/analysis

## Screenshots Index
| Step | Screenshot | What it shows |
|------|------------|---------------|
| 01 | screenshots/screenshot-01-system-info.png | Ubuntu OS version and network configuration verified (ip a, lsb_release). |
| 02 | screenshots/screenshot-02-disk-usage.png | Disk capacity check using df -h to confirm storage readiness. |
| 03 | screenshots/screenshot-03-wazuh-manager-running.png | Wazuh manager service enabled and active (systemctl status). |
| 04 | screenshots/screenshot-04-wazuh-indexer-running.png | Wazuh indexer running and stable (systemctl status). |
| 05 | screenshots/screenshot-05-wazuh-dashboard-running.png | Wazuh dashboard service running (systemctl status). |
| 06 | screenshots/screenshot-06-dashboard-connection-attempt.png | Initial dashboard access attempt and troubleshooting (localhost). |
| 07 | screenshots/screenshot-07-successful-wazuh-install.png | Successful installation output and access details (redacted if needed). |
| 08 | screenshots/screenshot-08-wazuh-dashboard-access.png | Successful Wazuh dashboard login/access in browser. |
| 09 | screenshots/screenshot-09-core-wazuh-running.png | Post-install validation of wazuh-manager running. |
| 10 | screenshots/screenshot-10-deploying-new-agent.png | Wazuh UI showing new agent deployment options. |
| 11 | screenshots/screenshot-11-enroll-windows11-endpoint.png | Windows agent enrollment/auth flow via PowerShell. |
| 12 | screenshots/screenshot-12-final-enrollment-confirmation.png | Wazuh dashboard shows agent active and connected. |
| 13 | screenshots/screenshot-13-windows-failed-auth-event-detected.png | Security alerts list showing events from Ubuntu and Windows agent. |
| 14 | screenshots/screenshot-14-alert-details-expanded-metadata.png | Expanded alert metadata view for investigation. |
| 15 | screenshots/screenshot-15-apparmor-privilege-violation-triggered.png | AppArmor DENIED event detected (host-based security). |
| 16 | screenshots/screenshot-16-alert-analysis-and-rule-details.png | Rule/alert detail view showing fields, source, and rule context. |


## Key Results
- Wazuh SIEM stack deployed successfully and services validated as running
- Windows 11 endpoint enrolled and reporting to the manager
- Security alerts generated and investigated through dashboard event details

## Notes
Sensitive values (passwords/keys) were not included in public artifacts. Screenshots were reviewed for redaction where necessary.
