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
  - create and configure storage account
    * Secure transfer (HTTPS) enabled by default
    * Cannot change performance tier once SA is created
  - generate shared access signature
    * Two types of SAS: (1) account-level SAS, (2) service-level SAS
    * Account-level SAS uses access keys for access. Allows full-access to entire storage account
    * Service-level SAS uses stored access policies (SAP)
    * SAP provides granular access to resources and can be deleted to revoke access w/out re-generating SA account access keys
  - implement Azure AD authentication for storage
  - install and use Azure Storage Explorer
  - manage access keys
  - monitor activity log by using Azure Monitor logs
  - implement Azure storage replication
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
  - manage and troubleshoot Azure AD Connect
  - troubleshoot password sync and writeback
	
## Implement solutions that use virtual machines (VM)
  - provision VMs
  - create Azure Resource Manager templates
  - configure Azure Disk Encryption for VMs
  - implement Azure Backup for VMs
  
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
    * Strong
    * Bounded Staleness
    * Session
    * Consistent Prefix
    * Eventual

## Develop solutions that use a relational database
  - provision and configure relational databases
  - configure elastic pools for Azure SQL Database
  - implement Azure SQL Database managed instances
    * [SQL Managed Instances](https://docs.microsoft.com/en-us/azure/azure-sql/managed-instance/sql-managed-instance-paas-overview#database-migration)
  - create, read, update, and delete data tables by using code
