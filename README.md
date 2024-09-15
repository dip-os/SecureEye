# SecureEye
A SIEM + SOAR solution
![alt text](https://github.com/dip-os/SecureEye/blob/main/SecureEye-SOC-Sub-Suvadip/secureEye.png?raw=true)
## SecureEye: Wazuh SIEM Integration with Shuffle, DFIR-IRIS, and VirusTotal
## Overview
SecureEye is an advanced security solution that integrates multiple tools to create a seamless workflow for threat detection, incident response, and active remediation. It leverages Wazuh for Security Information and Event Management (SIEM), Shuffle for automated workflows, DFIR-IRIS for incident response case management, and VirusTotal for malware analysis and IP blocking.



## How it Works
1. Log and Event Collection (Wazuh)
2. Workflow Automation (Shuffle)
3. Incident Response (DFIR-IRIS)
4. Active Threat Response (VirusTotal)

## Features
Real-time Log Collection: Collect logs from multiple sources via Wazuh SIEM.
Automated Workflows: Use Shuffle to create automated workflows for incident alerts.
Case Management: Create and manage cases for different rule IDs via DFIR-IRIS.
Active Response: Automatically block suspicious IPs and delete malicious files using VirusTotal integrations.
Scalable Solution: Designed to handle a wide variety of environments and multiple log sources.

## Architecture
1. Wazuh SIEM
Collects and analyzes security logs and events from multiple sources.
Provides a unified dashboard for monitoring security threats.
2. Shuffle Webhook
Automates the process of responding to Wazuh alerts by creating workflows.
Integration with Wazuh allows you to repeat back alerts and handle various incidents automatically.
3. DFIR-IRIS
Connects to Shuffle to create new cases when specific rule IDs are triggered.
Enables the tracking and management of incident response activities.
4. VirusTotal Integration
Active response mechanism to block suspicious IP addresses and delete malicious files based on Wazuh alerts.
Uses VirusTotal API for malware detection and analysis.

## Technologies Used
Wazuh: Open-source security monitoring and SIEM solution.
Shuffle: Automation tool for security operations.
DFIR-IRIS: Incident response case management tool.
VirusTotal: Online service that analyzes files and URLs for viruses and malware.
Docker: Containerization platform used to deploy components.
Webhook: Communication between Wazuh and Shuffle for real-time alerting.
