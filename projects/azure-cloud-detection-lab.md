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
<img width="2484" height="930" alt="image" src="https://github.com/user-attachments/assets/fbcf5e9f-f226-4a18-8a27-cabdbb9c16cd" />


---

### 3. Configuring Sentinel
Enabled **Azure Sentinel** on the workspace and created custom analytics rules.
<img width="2440" height="1177" alt="image" src="https://github.com/user-attachments/assets/10241da2-6ea2-46db-a820-a56ad86bc63b" />


---

### 4. Detection Testing
I simulated brute force login attempts on the VM. Sentinel generated alerts as expected.
<img width="1873" height="346" alt="image" src="https://github.com/user-attachments/assets/f2de8364-0d3d-4daa-86c1-7ad4ace37aab" />


---

### 5. Building the Attack Map
I created a geolocation based **attack map** in Azure Sentinel to visualize where incoming attacks originated.
<img width="1655" height="988" alt="Screenshot 2025-08-22 113640" src="https://github.com/user-attachments/assets/56d252f1-c636-4951-aafa-fbfdabbb13ca" />



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


