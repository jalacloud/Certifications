// Collection link: [SC200 Renewal Prep](https://learn.microsoft.com/en-us/collections/kkx7a2tqkk14yj)

# Microsoft SC-200 Renewal Study Notes


### Threat Analytics

Highest exposure—lists threats with the highest exposure levels first. the exposure level of a threat is calculated using two pieces of information: how severe the vulnerabilities associated with the threat are, and how many devices in your organization could be exploited by those vulnerabilities.


## Create and manage Microsoft Sentinel workspaces

[link](https://learn.microsoft.com/en-us/training/modules/create-manage-azure-sentinel-workspaces/)

* Microsoft Sentinel requires a Log Analytics Workspace.
* The Microsoft Sentinel solution is installed in a Log Analytics Workspace (LAW).
* The single most important option when creating a new Log Analytics Workspace is the region. The region specifies the location where the log data resides.

The three implementation options:

1. Single-Tenant with a single Microsoft Sentinel Workspace
2. Single-Tenant with regional Microsoft Sentinel Workspaces
3. Multiple tenants

#### Use the same log analytics workspace as Microsoft Defender for Cloud
Use the same workspace for both Microsoft Sentinel and Microsoft Defender for Cloud, so that all logs collected by Microsoft Defender for Cloud can also be ingested and used by Microsoft Sentinel. The default workspace created by Microsoft Defender for Cloud won't appear as an available workspace for Microsoft Sentinel.

### Types of Analytics Rules
* Scheduled Query Rule
* Microsoft Incident Creation Rule
* Near Real Time (NRT) Rule 
* Fusion Rule (_Cannot be edited/modified_)
