# wazuh-siem-lab
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
(Replace this line with your screenshot table + descriptions.)

## Key Results
- Wazuh SIEM stack deployed successfully and services validated as running
- Windows 11 endpoint enrolled and reporting to the manager
- Security alerts generated and investigated through dashboard event details

## Notes
Sensitive values (passwords/keys) were not included in public artifacts. Screenshots were reviewed for redaction where necessary.
