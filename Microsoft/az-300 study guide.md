# Microsoft Azure Architect Technologies (az-300)

# 1. Deploy and configure infrastructure (40-45%)
## Analyze resource utilization and consumption
  - configure diagnostic settings on resources
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
  - create and configure storage account
  - generate shared access signature
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
  
# Implement workloads and security (25-30%)
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
  - configure access to Azure resources by assigning roles
  - configure management access to Azure
  - troubleshoot RBAC
  - implement Azure Policies
  - assign RBAC Roles
