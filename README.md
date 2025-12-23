# Wazuh SIEM – Windows Authentication Monitoring Lab

## Overview
This project demonstrates a hands-on SIEM lab using **Wazuh** to monitor and analyze **Windows authentication events**.  
The lab focuses on collecting, validating, and investigating Windows Security Event Logs, with a specific emphasis on **failed logon attempts (Event ID 4625)**.

This project simulates a basic **SOC analyst workflow**, including agent deployment, log verification, and security event analysis.

---

## Lab Environment
- **SIEM Platform:** Wazuh (All-in-One)
- **Endpoint:** Microsoft Windows 10
- **Virtualization:** VirtualBox
- **Network Mode:** Host-Only Adapter
- **Log Source:** Windows Security Event Logs

---

## Objectives
- Deploy and configure a Wazuh agent on a Windows endpoint
- Verify successful agent onboarding and connectivity
- Collect Windows Security Event Logs
- Analyze authentication-related events using Wazuh Discover
- Detect failed logon attempts (Event ID 4625)

---

## Agent Deployment
The Wazuh agent was installed on a Windows 10 virtual machine and configured to communicate with the Wazuh manager.

Successful onboarding was confirmed by:
- Agent appearing in the Wazuh dashboard
- Agent status showing as **Active**
- Continuous log ingestion from the endpoint

---

## Log Collection Validation
Windows Security Event Logs were successfully collected and indexed by Wazuh.

This confirms:
- Proper agent configuration
- Successful communication between the agent and Wazuh manager
- Accurate parsing of Windows event data

---

## Authentication Event Analysis (Event ID 4625)

### Query Used

Event ID **4625** represents a **failed logon attempt** in Windows.

Using the Discover feature, failed authentication events were identified and reviewed.

---

## Analysis

The collected authentication events provide detailed security-relevant information such as:
- Target username
- Source IP address
- Authentication package
- Logon process
- Event timestamp

This data allows SOC analysts to investigate suspicious authentication behavior and identify potential brute-force or unauthorized access attempts.
---

## Findings
- The Windows agent was successfully deployed and remained active
- Windows Security Event Logs were collected without errors
- Failed login attempts (Event ID 4625) were detected and analyzed
- The lab demonstrates a foundational SOC monitoring and investigation workflow

---

## Conclusion
This project confirms the effectiveness of Wazuh as a SIEM solution for monitoring Windows authentication events.  
It provides hands-on experience in agent deployment, log validation, and security event analysis—key skills for SOC and blue-team roles.

---

## Screenshots
All screenshots related to this project are stored separately in the **screenshots/** directory.

---

## Report Documentation

A detailed technical report was prepared to document this project in a structured and formal format.

The report includes:
- Project objectives and environment setup
- Wazuh server and Windows agent deployment steps
- Log collection and validation process
- Analysis of Windows authentication events
- Investigation of failed logon attempts (Event ID 4625)
- Key findings and security observations

The report is intended to demonstrate practical SOC analysis skills, incident investigation methodology, and hands-on experience with SIEM tools.

The full report is provided separately as a Word document.
