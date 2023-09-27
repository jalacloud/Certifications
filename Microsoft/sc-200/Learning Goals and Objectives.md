# SC-200 Microsoft Security Operations Analyst
### Learning Goals and Objectives (LGO)

## 1 - Mitigate threats using Microsoft 365 Defender (25–30%) 
  - https://learn.microsoft.com/en-us/users/jason-7862/collections/xk4zarzp0ngdrp
  - https://learn.microsoft.com/en-us/training/paths/sc-200-mitigate-threats-using-microsoft-365-defender/
  - https://learn.microsoft.com/en-us/microsoft-365/security/defender/advanced-hunting-overview?view=o365-worldwide


## 1.1 Mitigate threats to the productivity environment by using Microsoft 365 Defender 
  • Investigate, respond, and remediate threats to Microsoft Teams, SharePoint, and OneDrive 
  • Investigate, respond, and remediate threats to email by using Microsoft Defender for Office 365

    Preset security policies [‘built-in’, ‘standard’, ‘strict’]
    Exchange Online Protection (EOP) policies work together with Office 365 policies.

  - https://mslearn.cloudguides.com/guides/Protect%20your%20organization%20with%20Microsoft%20365%20Defender
 
  • Investigate and respond to alerts generated from Data Loss Prevention policies
  
    Identify sensitive information across multiple platforms.
    Identify information inside a document, for example, credit card numbers.
    **Prevent** accidental sharing.
    Monitor and protect sensitive information.
    DLP alerts and reports based on associated policies.
    DLP policies can be applied across the Microsoft product suite.
    Restrict third-party access/sharing: Google/G-Suite, Box, Dropbox…etc.

  - https://compliance.microsoft.com/datalossprevention/overview

  • Investigate and respond to alerts generated from insider risk policies 

    Policy / Scope
    Alerts (created inside the policies)
    Triage (evaluation and assignment)
    Investigate
    Action
    
    Insider Risk Management Admin role is required for creating, assigning and managing Insider Risk Management (IRM) policies/alerts.



  • Identify, investigate, and remediate security risks by using Microsoft Defender for Cloud Apps 
  • Configure Microsoft Defender for Cloud Apps to generate alerts and reports to detect threats

    Defender for Cloud Apps is converged into the M365 Defender portal—no dedicated portal for cloud apps (MCAS). 
    Enable alerts within new policies that you create in the Microsoft Defender portal.

## 1.2 Mitigate endpoint threats by using Microsoft Defender for Endpoint 
• Manage data retention, alert notification, and advanced features 
• Recommend security baselines for devices 
• Respond to incidents and alerts 
• Manage automated investigations and remediations
Attack Surface Reduction (ASR)
Automated Incident Response (AIR)
• Assess and recommend endpoint configurations to reduce and remediate vulnerabilities by 
using Microsoft's threat and vulnerability management solution 
• Manage endpoint threat indicators 
Mitigate identity threats 
• Identify and remediate security risks related to events for Microsoft Azure Active Directory 
(Azure AD), part of Microsoft Entra 
• Identify and remediate security risks related to Azure AD Identity Protection events 
• Identify and remediate security risks related to Azure AD Conditional Access events 
• Identify and remediate security risks related to Active Directory Domain Services using Microsoft Defender for Identity 

### **Microsoft 365 Defender for Endpoint**

License requirement: Microsoft Defender for Endpoint Plan 2
Separate license from Microsoft Enterprise Mobility + Security (EMS) E5

Device onboarding
Create a role to administer and manage Microsoft Defender for Endpoint

Attack Surface Reduction (ASR) Rules
Exploit Protection
Application Control

Developer Mindset vs. Security Mindset

Assets
Devices (device inventory)
Identities

Behavioural blocking stops threats based on their behaviour.
Enabled in Defender for Endpoint.
Next-Generation Protection Feature

Defender for Endpoint = Identities, Emails, Applications, and Endpoints

Applications Controls
Client behavioural blocking
Detects suspicious behaviours on devices
Can be remediated automatically
Stops attacks as they occur


## 1.3 Manage extended detection and response (XDR) in Microsoft 365 Defender 
• Manage incidents across Microsoft 365 Defender products 
• Manage investigation and remediation actions in the Action Center 
• Perform threat hunting 
• Identify and remediate security risks using Microsoft Secure Score 
• Analyze threat analytics 
• Configure and manage custom detections and alerts 

### DOMAIN 1 STUDY NOTES:

Zero-hour Auto Purge (ZAP) - retroactively detects and remediates malicious malware phishing, spam or malware threats delivered by email to Microsoft 365 Exchange Online mailboxes. 
ZAP doesn’t work for standalone Exchange Online Protection (EOP) environments that protect on-premises exchange mailboxes.
Kusto Query Language (KQL) is used across multiple products, including Sentinel, Log Analytics and MS Defender for Endpoint.
Correlation across MS products is key to successfully defending/mitigating threats.

### **Microsoft 365 Defender**

  - Microsoft 365 Defender Portal - correlated view of all incidents across Microsoft Azure estate.
  - MS Defender enables cross-domain threat correlation (CDTC)
  - MS Defender is also a type of cloud workload protection platform (CWPP)

  - Microsoft 365 Defender can automatically detect new anomalies by correlating alert events from different Microsoft Security products.
  - Incidents are based on related alerts.
  - Clues and alerts are aggregated.
  - An incident can be categorised as Active or Resolved.
  - Can manage incidents across devices, users and mailboxes.
  - M365 Defender is aligned with the MITRE ATT&CK framework.

  - Advanced Hunting is a query-based threat-hunting tool. Explore up to 30 days of raw data.
  - Based on two types of data/information:
      1. Event or Activity Data
      2. Entity Data

### **KQL**
  - The “Project” parameter is used to select specific columns from tables.
  - Auto-generate queries using built-in query examples.

### **M365 Defender for Office 365**

Cloud-based email filtering service.
Industry-leading protection suite - 6.5 trillion signals from email alone.
Actionable Insights
Automated Response capabilities

Exchange Online Protection (EOP) policies:
Standard Protection (suitable for most users)
Strict Protection (for high-value (HV) targets, increased protection)
Preset security policies are applied to users after you assign the Standard or Strict preset protection profiles to your users.

M365 Defender investigations and threat explorer tabs rely on data from the policies & rules that you have pre-configured for alerts and detections.

### **M365 Defender for Identity**

Monitors user behaviour and user activities
Reduction of attack surface by providing detailed security reports and user analytics
Requires sensors to be installed and deployed on domain controller (DC) systems
  - Sensors require the domain admin credentials to be provided in the Defender portal
  - Installation of the sensors requires a valid access key to be provided during installation
User Risk
  - Caused when user identity is compromised
  - Unusual user behaviours
  - Leaked credentials via spam email or phishing email
Sign-In Risk
  - Unfamiliar Sign-in properties
  - Atypical Travel
  - Malware Linked IP addresses
  - Anonymous IP address


### **Microsoft 365 Defender for Cloud Apps**

  - https://learn.microsoft.com/en-us/defender-cloud-apps/what-is-defender-for-cloud-apps

Phases of Cloud App Security
Data Discovery
Classify Sensitive Information
Personal label
Public
General
Confidential data
Highly Confidential data
Protecting the data 
Monitor and Report




## 2 - Mitigate threats using Microsoft Defender for Cloud (20–25%) 

Microsoft Cloud App Security (MCAS) portal is now converged into the Microsoft 365 Defender Portal. 

## 2.1 Implement and maintain cloud security posture management and workload protection 
• Plan and configure Microsoft Defender for Cloud settings, including selecting the target 
subscriptions and workspaces 
• Configure Microsoft Defender for Cloud roles 
• Assess and recommend cloud workload protection 
• Identify and remediate security risks using the Microsoft Defender for Cloud Secure Score 
• Manage policies for regulatory compliance 
• Review and remediate security recommendations 

## 2.2 Plan and implement the use of data connectors for ingestion of data sources in Microsoft Defender for Cloud 
• Identify data sources to be ingested for Microsoft Defender for Cloud 
• Configure automated onboarding for Azure resources 
• Connect multi-cloud and on-premises resources 
• Configure data collections 

## 2.3 Configure and respond to alerts and incidents in Microsoft Defender for Cloud 
• Validate alert configuration 
• Set up email notifications 
• Create and manage alert suppression rules 
• Design and configure workflow automation in Microsoft Defender for Cloud 
• Remediate alerts and incidents by using Microsoft Defender for Cloud recommendations 
• Manage security alerts and incidents 
• Analyze Microsoft Defender for Cloud threat intelligence reports 
• Manage user data discovered during an investigation 

## 3 - Mitigate threats using Microsoft Sentinel (50–55%) 
## 3.1 Design and configure a Microsoft Sentinel workspace 
• Plan a Microsoft Sentinel workspace 
• Configure Microsoft Sentinel roles 
• Design and configure Microsoft Sentinel data storage 
• Implement and use Content hub, repositories, and community resources 

## 3.2 Plan and implement the use of data connectors for ingestion of data sources in Microsoft Sentinel 
• Identify data sources to be ingested for Microsoft Sentinel 
• Identify the prerequisites for a Microsoft Sentinel data connector 
• Configure and use Microsoft Sentinel data connectors 
• Configure Microsoft Sentinel data connectors by using Azure Policy 
• Configure Microsoft Sentinel connectors for Microsoft 365 Defender and Microsoft Defender for Cloud 
• Design and configure Syslog and CEF event collections 
• Design and configure Windows Security event collections 
• Configure custom threat intelligence connectors 
## 3.3 Manage Microsoft Sentinel analytics rules 
• Design and configure analytics rules 
• Activate Microsoft security analytics rules 
• Configure built-in scheduled queries 
• Configure custom scheduled queries 
• Define incident creation logic 
• Manage and use watchlists 
• Manage and use threat indicators 

## 3.4 Perform data classification and normalisation 
• Classify and analyse data by using entities 
• Create custom logs in Azure Log Analytics to store custom data 
• Query Microsoft Sentinel data by using Advanced SIEM Information Model (ASIM) parsers 
• Develop and manage ASIM parsers 

## 3.5 Configure Security Orchestration, Automation, and Response (SOAR) in Microsoft Sentinel 
• Configure automation rules 
• Create and configure Microsoft Sentinel playbooks 
• Configure alerts and incidents to trigger automation 
• Use automation to remediate threats 
• Use automation to manage incidents 

## 3.6 Manage Microsoft Sentinel incidents 
• Triage incidents in Microsoft Sentinel 
• Investigate incidents in Microsoft Sentinel 
• Respond to incidents in Microsoft Sentinel 
• Investigate multi-workspace incidents 
• Identify advanced threats with User and Entity Behavior Analytics (UEBA) 

## 3.7 Use Microsoft Sentinel workbooks to analyze and interpret data 
• Activate and customize Microsoft Sentinel workbook templates 
• Create custom workbooks
• Configure advanced visualizations 
• View and analyze Microsoft Sentinel data using workbooks 
• Track incident metrics using the security operations efficiency workbook 

## 3.8 Hunt for threats using Microsoft Sentinel 
• Create custom hunting queries 
• Run hunting queries manually 
• Monitor hunting queries by using Livestream 
• Configure and use MSTICPy in notebooks 
• Perform hunting by using notebooks 
• Track query results with bookmarks 
• Use hunting bookmarks for data investigations 
• Convert a hunting query to an analytical rule
