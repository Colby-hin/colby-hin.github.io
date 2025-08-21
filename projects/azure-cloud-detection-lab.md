# Azure Cloud Detection Lab

## Overview
In this project, I set up **Azure Sentinel (SIEM)** and configured it to detect malicious activity inside a cloud environment.  
This lab demonstrates my skills in log collection, threat detection, and incident response.

---

## Objectives
- Deploy a Windows VM in Azure
- Connect VM logs to Azure Log Analytics
- Set up Azure Sentinel (SIEM)
- Create detection rules for suspicious activity
- Investigate alerts using KQL queries

---

## Steps

### 1. Deploying the VM
I created a Windows Server VM inside Azure and enabled logging.
![VM Deployment Screenshot](../images/vm-deployment.png)

---

### 2. Connecting Logs
I connected the VM to **Azure Log Analytics Workspace** and verified event logs were being ingested.
![Log Analytics Screenshot](../images/log-analytics.png)

---

### 3. Configuring Sentinel
Enabled **Azure Sentinel** on the workspace and created custom analytics rules.
![Sentinel Setup Screenshot](../images/sentinel-setup.png)

---

### 4. Detection Testing
I simulated brute force login attempts on the VM. Sentinel generated alerts as expected.
![Alert Screenshot](../images/sentinel-alert.png)

---

## Results
- Successfully ingested logs from VM → Sentinel.  
- Created detection rules for failed RDP logins.  
- Queried and investigated alerts with **KQL**.  

---

## Skills Demonstrated
- SIEM Implementation & Log Analysis  
- Threat Detection & Response  
- KQL Querying  
- Incident Investigation  

---

## Next Steps
- Add additional detection rules  
- Integrate threat intelligence feeds  
- Automate response with playbooks  
