# Microsoft Azure Architect Technologies (az-300)

# 1. Deploy and configure infrastructure (40-45%)
## Analyze resource utilization and consumption
  - configure diagnostic settings on resources
    * Enable __guest-level monitoring__ for virtual machines
    * Requires a "diagnostics storage account" to be created
  - create baseline for resources
    * [security baselines in Azure](https://docs.microsoft.com/en-us/learn/modules/create-security-baselines/)
  - create and test alerts
  - analyze alerts across subscription
  - analyze metrics across subscription
  - create action groups
  - monitor for unused resources
    * Azure Adviser provides recommendations for unused/under utilised resources.
  - monitor spend
    * Cost analysis feature: __subscription -> cost management -> cost analysis__
  - report on spend
  - utilize Log Search query functions
  - view alerts in Azure Monitor logs
  - visualize diagnostics data using Azure Monitor Workbooks

## Create and configure storage accounts
  - configure network access to the storage account
    * Access from public/private networks are allowed by default
    * Control access by using the __resource firewall__ within the storage account
    * Allow access from: __selected networks__ to lock down access to specific VNets
    * Subnets configured with the "Microsoft.Storage" service endpoint can __privately__ access Azure Storage without traversing the  public internet.
  - create and configure storage account
    * Secure transfer (HTTPS) enabled by default
    * Cannot change performance tier once SA is created
    * Soft Delete can be enabled for __File Shares__
      * Retention configured by user/admin
    * Configue soft-delete for Blob storage in Azure portal -> Blob Service -> __Data Protection__ "Enable Soft Delete"
    * Azure Storage supports using Azure Active Directory (Azure AD) to authorise requests to Blob and Queue storage.
  - generate shared access signature
    * Three (3) types of SAS:
      * __account-level SAS__: Uses account keys for access. Grants read/write/delete operations on blobs/tables/queues/files. Re-gen keys if sas is leaked. Can also grant permissions to services (blob/queue/table/files) not permitted with a service SAS.
      * __service-level SAS__: Granular access. Uses stored access policies (SAP). Access to specific services - more control over access.
      * __user-delegation SAS__: secured with Azure AD credentials and also by the permissions specified for the SAS. User delegation SAS applies to __Blob__ storage only.
      * [Types of SAS](https://docs.microsoft.com/en-us/azure/storage/common/storage-sas-overview)
    * Account-level SAS uses access keys for access. Scope of access applies to entire storage account and services within the SA.
    * Service-level SAS uses stored access policies (SAP).
    * SAP provides granular access to resources and can be deleted to revoke access w/out re-generating SA account access keys.
  - implement Azure AD authentication for storage
    * Managed Identities for Azure resources can authorise access to blob and queue data using Azure AD credentials.
    * Service Principals __must__ be assigned an RBAC role that grants access to blob or queue data in Azure Storage.
    * [Authorise access to blobs/queues using AAD](https://docs.microsoft.com/en-us/azure/storage/common/storage-auth-aad)
  - install and use Azure Storage Explorer
  - manage access keys
  - monitor activity log by using Azure Monitor logs
  - implement Azure storage replication (6 types)
    * Locally Redundant Storage (LRS)
    * Zone-Redundant Storage (ZRS)
    * Geo-Redundant Storage (GRS)
    * Geo-Zone Redundant Storage (GZRS)
    * Read-Access Geo-Redundant Storage (RA-GRS) -> Not supported by Azure File Shares
    * Read-Access Geo-Zone Redundant Storage (RA-GZRS)
  - implement Azure storage account failover

## Create and configure a VM for Windows and Linux
  - configure high availability
    * Availability Sets; update domains, and fault domains.
    * VMs MUST be located within the same region and resource group as the availability set.
    * Virtual Machine Scale Sets (VMSS).
  - configure monitoring
  - configure networking
  - configure storage
  - configure virtual machine size
  - implement dedicated hosts
  - deploy and configure scale sets

## Automate deployment of VMs
  - modify Azure Resource Manager template
  - configure location of new VMs
  - configure VHD template
  - deploy from template
  - save a deployment as an Azure Resource Manager template
  - deploy Windows and Linux VMs
  
## Create connectivity between virtual networks
  - create and configure Vnet peering
  - create and configure Vnet to Vnet connections
  - verify virtual network connectivity
  - create virtual network gateway

## Implement and manage virtual networking
  - configure private IP addressing
  - configure public IP addresses
  - create and configure network routes
  - create and configure network interface
  - create and configure subnets
  - create and configure virtual network
  - create and configure Network Security Groups and Application Security Groups
  
## Manage Azure Active Directory
  - add custom domains
  - configure Azure AD Identity Protection
  - configure Azure AD Join
  - configure self-service password reset
  - implement conditional access policies
  - manage multiple directories
  - perform an access review
	
## Implement and manage hybrid identities
  - install and configure Azure AD Connect
  - configure federation
  - configure single sign-on
    * [Configure SSO](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso-quick-start)
    * Enable SSO option in Azure AD Connect only available for: Pass-through Authentication (PTA) and Password Hash Synchronisation (PHA) authentication method(s).
  - manage and troubleshoot Azure AD Connect
  - troubleshoot password sync and writeback
	
## Implement solutions that use virtual machines (VM)
  - provision VMs
  - create Azure Resource Manager templates
  - configure Azure Disk Encryption for VMs
    * Requires enabling Azure Key Vault to be used for VM Disk Encryption
    * Enabled in Azure Key Vault -> __advanced key vault access policy settings__
  - implement Azure Backup for VMs
    * Uses "Backup Policies" to configure backup schedules and retention times for backed up resources (VMs)
    * __Soft Delete__ is enabled by default for Azure Backup / Recovery Services Vault (RSV)
    * Soft Delete for Azure Backup/RSV has a retention period of __14 Days__
  
# 2. Implement workloads and security (25-30%)
## Migrate servers to Azure
  - migrate servers using Azure Migrate
    * [Azure Migrate](https://docs.microsoft.com/en-us/azure/migrate/migrate-services-overview)
    * [VMware support matrix](https://docs.microsoft.com/en-us/azure/site-recovery/vmware-physical-azure-support-matrix)
    * [Hyper-V support matrix](https://docs.microsoft.com/en-us/azure/site-recovery/hyper-v-azure-support-matrix#azure-vm-requirements)
	
## Configure serverless computing
  - create and manage objects
  - manage a Logic App resource
  - manage Azure Function app settings
    * [Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference)
    * Config for the Azure Functions app is contained within the __functions.json file.__
    * Uses __consumption plan__ by default - resources added dynamically
    * When using app service plan, you manage the scaling of your function app
    * Uses {appname}.azurewebsites.net namespace
    * Can be published using code or docker container
  - manage Event Grid
    * Uses publish/subscribe model.
    * Does not need to constantly poll for events.
    * Does not waste CPU resources by constantly polling.
  - manage Service Bus
    * Message queuing service
    * Uses __dead-letter queuing__ to store unprocessed messages for a period of time (TTL).
    * Uses __single message queue__ for one-to-one messaging
    * Uses __topics__ for one-to-many message applications
	
## Implement application load balancing
  - configure application gateway
    * Provides layer-7 load-balancing functionality
    * Can be deployed as WAF for web application vuln detection/protection.
    * Can perform URL/path-based routing.
    * Supports SSL/TLS off-loading.
    * Same port (e.g. 80) cannot be used for both public and private listeners.
    * __Only one public IP address is supported on an application gateway__
  - configure Azure Front Door service
  - configure Azure Traffic Manager

## Integrate on premises network with Azure virtual network
  - create and configure Azure VPN Gateway
    * Microsoft recommend __/27__ (or larger) for configuring VPN _GatewaySubnets_ when trying to save address space
    * /27 is the smallest option possible for GatewaySubnet subnet configuration
    
  - create and configure site to site VPN
  - configure ExpressRoute
  - configure Virtual WAN
  - verify on premises connectivity
  - troubleshoot on premises connectivity with Azure

## Implement multi factor authentication
  - configure user accounts for MFA
  - configure fraud alerts
  - configure bypass options
  - configure trusted IPs
  - configure verification methods

## Manage role-based access control
  - create a custom role
    * Replicate existing role: __Get-AzRoleDefinition__ -Name "Reader" | __ConvertTo-Json__ | Out-File C:\<path-to-file.json>
    * Use __New-AzRoleDefinition__ -InputFile "C:\CustomRoles\{myCustomRole}.json
    * Get-AzRoleDefinition - lists all custom roles created
    * [Custom Role Tutorial](https://docs.microsoft.com/en-us/azure/role-based-access-control/tutorial-custom-role-powershell)
  - configure access to Azure resources by assigning roles
  - configure management access to Azure
    * Management access using: Conditional Access Policies, Azure MFA, Azure Identitiy Protection (IdP)
  - troubleshoot RBAC
  - implement Azure Policies
  - assign RBAC Roles

# 3. Create and deploy apps (5-10%)
## Create web apps by using PaaS
  - create an Azure app service Web App
  - create documentation for the API
  - create an App Service Web App for Containers
  - create an App Service background task by using WebJobs
  - enable diagnostics logging

## Design and develop apps that run in containers
  - configure diagnostic settings on resources
  - create a container image by using a Dockerfile
  - create an Azure Kubernetes Service
  - publish an image to the Azure Container Registry
  - implement an application that runs on an Azure Container Instance
  - manage container settings by using code

# 4. Implement authentication and secure data (5-10%)
## Implement authentication
  - implement authentication by using certificates, forms-based authentication, tokens, or Windows-integrated authentication
  - implement multi-factor authentication by using Azure AD
  - implement OAuth2 authentication
  - implement Managed Identities for Azure resources Service Principal authentication

## Implement secure data solutions
  - encrypt and decrypt data at rest and in transit
  - encrypt data with Always Encrypted
  - implement Azure Confidential Compute
    * Use __DC series__ virtual machines. DC series VMs support confidential compute. 
  - implement SSL/TLS communications
  - create, read, update, and delete keys, secrets, and certificates by using the KeyVault API

# 5. Develop for the cloud and for Azure storage (15-20%)
## Configure a message-based integration architecture
  - configure an app or service to send emails
    * Can configure an Azure Logic App (workflow app) to send emails based on events generated from Event Grid
    * Logic Apps can be used with Azure Event Grid
    * SendGrid is a feature/service that can send generated emails <-- __find more detailed info on this__ 
  - configure Event Grid
  - configure the Azure Relay service
  - create and configure a Notification Hub
  - create and configure an Event Hub
  - create and configure a Service Bus

## Develop for autoscaling
  - implement autoscaling rules and patterns (schedule, operational/system metrics)
  - implement code that addresses singleton application instances
  - implement code that addresses transient state

## Develop solutions that use Cosmos DB storage
  - create, read, update, and delete data by using appropriate APIs
  - implement partitioning schemes
  - set the appropriate consistency level for operations
    * Consistency levels can be overwritten through the SDK for a while client or per-request.
    * Default consistency levels are configured at the CosmosDB Account level.
    * Consistency levels are __region agnostic__ and are guaranteed for __all__ read operations.
    * __1. Strong__: reads are guaranteed to return most recent committed version of item.
    * __2. Bounded Staleness__: consistent to an agreed amaount: 
      * reads might lag behind writes by at most [number] version of an item;
      * reads might lag behind writes for an [amount] amount of time
    * __3. Session__: reads guaranteed to honor writes for a given client session.
    * __4. Consistent Prefix__: guarantees that reads NEVER see out-of-order writes.
    * __5. Eventual__: no guarantee about order of reads; replicas with _eventually_ converge.
  - __Bonus Info:__
    * CosmosDB SQL API accounts support querying items using SQL as a JSON query
    * Provides low latency access to data items

## Develop solutions that use a relational database
  - provision and configure relational databases
  - configure elastic pools for Azure SQL Database
  - implement Azure SQL Database managed instances
    * [SQL Managed Instances](https://docs.microsoft.com/en-us/azure/azure-sql/managed-instance/sql-managed-instance-paas-overview#database-migration)
  - create, read, update, and delete data tables by using code
