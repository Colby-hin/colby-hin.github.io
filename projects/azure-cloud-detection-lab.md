# Azure Cloud Detection Lab

## Overview
In this project, I deployed a honeypot virtual machine in Azure, intentionally exposed to the public internet to attract and log malicious activity.
I set up Azure Log Analytics Workspace and integrated it with Azure Sentinel (SIEM) to collect and analyze security events.

---

## Objectives
- Deploy a Windows VM in Azure
- Connect VM logs to Azure Log Analytics
- Set up Azure Sentinel (SIEM)
- Create detection rules for suspicious activity
- Investigate alerts using KQL queries
- Develope an attack map dashboard showing attacker geolocations

---

## Steps

### 1. Deploying the VM
I created a Windows VM inside Azure and enabled logging.
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


### 5. Building the Attack Map
I created a geolocation based **attack map** in Azure Sentinel to visualize where incoming attacks originated.  

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


