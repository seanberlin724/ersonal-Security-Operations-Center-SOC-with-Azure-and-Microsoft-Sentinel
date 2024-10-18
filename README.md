# Personal Security Operations Center (SOC) with Azure and Microsoft Sentinel

## Objective
To develop a cloud-based Security Operations Center (SOC) using Azure Virtual Machines and Microsoft Sentinel to simulate real-world security monitoring and threat detection processes. This project aims to demonstrate the configuration of an SIEM system, focusing on monitoring Remote Desktop Protocol (RDP) access, creating detection rules, and generating alerts for potential security threats.


### Skills Learned
- Configuring cloud-based virtual machines (Azure VM)
- Setting up and managing a Security Information and Event Management (SIEM) system with Microsoft Sentinel
- Monitoring network traffic and RDP access for security incidents
- Creating and fine-tuning detection rules for real-time threat alerting
- Working with Log Analytics Workspace for centralized data ingestion and monitoring

### Tools Used
- **Azure** (Virtual Machines, Log Analytics Workspace)
- **Microsoft Sentinel** (SIEM system)
- **RDP** (Remote Desktop Protocol)
- **Custom detection rules** in Microsoft Sentinel
- **Log Analytics** for data ingestion and analysis

## Steps
### 1. Set up Azure Virtual Machine
- Created a Windows-based Virtual Machine in Azure, using the free trial credits for deployment.
- Exposed RDP (Remote Desktop Protocol) access to simulate potential attacks and generate security events for monitoring.
<img src="Images/1.png">

*Ref 1: Azure Virtual Machine Overview Screenshot*


### 2. Configure Microsoft Sentinel
- Deployed Microsoft Sentinel on Azure and linked it to the Log Analytics Workspace to begin ingesting security event logs from the VM.
- Connected the VM’s security logs to Sentinel using Data Connectors, enabling log collection for analysis.
<img src="Images/2.png">

*Ref 2: Microsoft Sentinel Dashboard Screenshot*

### 3. Create Custom Detection Rules for RDP Sign-ins
- Configured custom detection rules in Microsoft Sentinel to monitor and alert on successful RDP sign-ins.
- The rules triggered real-time alerts, allowing for immediate detection of suspicious login attempts.
<img src="Images/3a.png">

*Ref 3: Custom Detection Rule Setup Screenshot 1/2*

<img src="Images/3b.png">

*Ref 3: Custom Detection Rule Setup Screenshot 2/2*

### 4. Real-Time Alerts and Analytics
- Demonstrated real-time incident generation in Microsoft Sentinel by attempting RDP logins. The successful attempts were flagged and alerted by the custom detection rules set up in the previous step.
- Incidents were generated for both successful logins via RDP, simulating a real-world security scenario (i.e. brute force attack).
<img src="Images/4.png">

*Ref 4: Microsoft Sentinel Analytics Screenshot*

### 5. Log Analytics Workspace Configuration
- Linked the Azure Virtual Machine to the Log Analytics Workspace to centralize data collection.
- Optimized data ingestion and monitoring workflows, ensuring that security events from the VM were available for analysis in real-time.
<img src="Images/5a.png">

*Ref 5:  Microsoft Sentinel Incidents Screenshot*

<img src="Images/5b.png">

*Ref 5: Incident Details Screenshot*

### Future Enhancements
- Integrate threat intelligence indicators through API calls for more comprehensive security monitoring.
- Implement automation for responding to specific alerts, reducing the need for manual intervention.
