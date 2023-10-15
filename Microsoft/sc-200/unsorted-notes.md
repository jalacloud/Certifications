## Unsorted SC-200 Study Notes

Notes taken while going through Udemy course: https://udemy.com/course/sc-200-microsoft-security-operations-analyst-exam-prep 

#### Defender for Cloud Apps
- Provides Adaptive Network Hardening (ANH)
- Defender for cloud apps is enabled by default as soon as you create a new Azure web app


#### Defender for Storage
- Azure-native security
- Support for blob, data lake
- One-click deployment, no manual setup required.
- Detects suspicious access patterns
- Detects uploads of malicious content
- Hash reputation analysis
  
Workflow automation 
- used for creating automated actions to be taken when suspicious files/actions have been detected

#### Defender for Office 365
- Provides cloud-based email protection
- Can be enabled to protect Exchange Online cloud-hosted mailboxes
- Can be used in a hybrid deployment to protect messaging and control mail routing with a mix of on-premises and cloud mailboxes with Exchange Online Protection (EOP)
- Provides inbound email filtering
- Default anti-phishing policy in MDO 365 provides spoof protection and mailbox intelligence for all recipients
  - Impersonation protection and advanced features are not configured by default
  - To enable ALL protection features, modify the default anti-phishing policy or create additional anti-phishing policies
- Able to apply 'standard' or 'strict' level of protection to MDO 365 protection policies

Email protection policies:
  - Anti-spam
  - Anti-phishing
  - Anti-malware
  - Safe Attachments
  - Safe Links

Automated Investigation and Response (AIR)
- Uses a set of playbooks and triggers (alerts) to launch automated investigation and response activities
- Remediation actions in AIR include:
    - Soft delete email messages or clusters
    - Block URL (time-of-click)
    - Turn off external mail forwarding
    - Turn off delegation

#### [Defender for Identity](https://learn.microsoft.com/en-us/training/modules/m365-threat-safeguard/)

