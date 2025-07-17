AZ-900 - Microsoft Azure Fundamentals Certification

**Skills at a glance**

- Describe cloud concepts (25–30%)
- Describe Azure architecture and services (35–40%)
- Describe Azure management and governance (30–35%)

**Material from Microsoft Learn:**

**Describe cloud concepts (25-30%):**

- _What is Cloud computing?_

Delivery of computing services over the internet.

Includes VMs, storage, databases, and networking.

IoT, ML, and AI

- _Shared responsibility model_

On-prem – All customer

IaaS – Cloud provider has responsibility for physical infrastructure

PaaS/SaaS – Customer has responsibility for devices, accounts, and data, cloud provider for everything else.

- _Cloud models_

Private cloud – Used by a single entity. Greater cost.

Public cloud – Built, controlled, and maintained by a cloud provider. General public availability.

Hybrid cloud – Uses both public and private clouds in an inter-connected environment. Extra layer of security when choosing what goes on the public and private cloud parts.

Multi-cloud – Multiple public cloud providers used.

Azure Arc – Set of technologies that helps manage your cloud environment.

Azure VMware solution – Lets you run your VMware workloads in Azure with seamless integration.

- _Consumption-based model_

Capital expenditure (CapEx – one-time upfront fee) and Operational expenditure (OpEx – Renting a service)

Cloud computing is OpEx

Consumption-based model works off you pay for the resources you use and don’t for any resources not used.

- _High availability and scalability_

High availability – Resources are available when needed. Ensures maximum availability, regardless of disruptions or events that may occur.

Scalability – Ability to adjust resources to meet demand. When peak traffic is experience, resources can be scaled to accommodate.

Vertical scaling – Add more power to a machine – CPU, RAM.

Horizontal scaling – Adding more machines for resources – VMs, containers.

- _Reliability and predictability_

Reliability – Ability of a system to recover from failures and continue to function. Pillar of the Microsoft Azure Well-Architected Framework.

Predictability – Lets you move forward with confidence, whether performance predictability or cost predictability.

Performance – Predicting the resources needed to deliver a positive experience for your customers.

Cost – Predicting or forecasting the cost of the cloud spend.

- _Security and governance_

Maximum control of governance by customer – IaaS

Cloud provider takes on more governance – PaaS or SaaS

- _Manageability_

Management of the cloud – Automatically scale, deploy resources, monitor health, receive automatic alerts.

Management in the cloud – Through web portal, CLI, APIs, PowerShell

- _Infrastructure as a Service_

Maximum amount of control for your cloud resources

Lift and shift migration

Testing and development

- _Platform as a Service_

Middle ground between renting space in a datacentre (IaaS) and paying for a complete and deployed solution (SaaS).

Development framework

Analytics or business intelligence

- _Software as a Service_

Most complete cloud service model from a product perspective. With SaaS you’re essentially renting or using a fully developed application.

Least flexible but easiest to get up and running.

E-mail and messaging, business productivity applications, finance and expense tracking.

**Describe Azure architecture and services (35–40%):**

- _What is Microsoft Azure?_

Continually expanding set of cloud services that help you meet current and future business challenges.

- _Azure accounts_

Subscription needed for Azure

Free account – Free access to Azure products for 12 months, credit to use for first 30 days, access 25 products that are always free.

Free student account – Free access to Azure services for 12 months, credit to use in first 12 months, free access to certain software developer tools.

Microsoft learn sandbox – Temporary subscription assigned to you to complete modules.

- _Azure physical infrastructure_

Datacentres all around the world.

Grouped into Azure Regions or Azure Availability Zones that help with reliability for business-critical workloads.

Regions – Geographical area that contains at least one or multiple datacentres that are nearby, networked together with a low-latency network.

Availability zones – Physically separate datacentres within an Azure region. Used in isolation in case of disruption it can function on its own through high-fibre optic.

Region pairs – At least 300 miles away. Does this in case of a natural disaster at one site, it can failover to the other site.

Sovereign regions – Instances of azure that are isolated from the main instance of Azure. May need a sovereign region for compliance or legal purposes.

- _Azure management infrastructure_

Azure resources and resource groups – Grouping of resources. Easier to group resources together when applying actions instead of doing it individually.

Azure subscriptions – Provides you with authenticated and authorised access to Azure products and services.

Billing boundary – Determines how the account is billed for Azure. Multiple subscriptions and Azure will break it down per subscription so you can see where cost is going.

Access control boundary – Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organisational structurers and what can be provisioned where.

Azure management groups – A step above subscriptions where you can manage subscriptions and compliance. Mainly for larger organisations.

Organise subscriptions into containers called management groups and apply governance conditions. – Create a hierarchy and apply a policy or provide user access to multiple subscriptions.

10,000 management groups can be supported in a single directory.

A management group tree can support up to six levels of depth.

- _Azure virtual machines_

VMs provide total control of the OS, ability to run custom software, use custom hosting configurations

Scale of VMs in Azure.

VM scale sets allow Azure to configure a group of identical VMs.

VM availability sets allow VMs to stagger updates and have varied power preventing you from losing all your VMs in an event of power failure.

Use VMs during testing and development, running applications in the cloud, extending datacentre to the cloud, during disaster recovery.

VM resources include – Size, storage disks and networking.

- _Azure virtual desktop_

Desktop and application virtualisation service that runs on the cloud. Enables use of a cloud-hosted version of Windows from any location.

- _Azure containers_

Containers are a virtualisation environment that hold everything relevant such as software for an application to run.

Azure containers are PaaS solution. Allows you to upload your containers and then the service runs the container for you.

Containers Apps can load balance and scale.

Azure Kubernetes Service (AKS) is a container orchestration service. Manages the lifecycle of containers. Makes deployment easier.

- _Azure functions_

Serverless computing when the Infrastructure or Platform is not important.

Functions scale automatically based on demand.

- _Application hosting options_

Azure App Service – Enables you to build and host web apps, background jobs, mobile back-ends, and RESTful APIs n the programming language of your choice without managing the infrastructure.

Can host on web apps, API apps, WebJobs, and Mobile apps.

App service handles most of the infrastructure decisions such as deployment, endpoint security, scalability.

- _Azure virtual networking_

Azure virtual networks provides – isolation and segmentation, internet communications, communication between resources, filtering traffic.

- _Azure virtual private networks_

VPNs are encrypted tunnels within a network.

Azure VPN gateway instances are deployed in a dedicated subnet of the virtual network and enable the connectivity – to datacentres, individual devices, networks.

Policy-based VPN gateways specify statically the IP address of packets that should be encrypted through each tunnel.

Route-based gateways, IPSec tunnels are modelled as a network interface or virtual tunnel interface.

Active/standby – VPN gateways are deployed as this. Even if one gateway can be seen only.

Active/active – Assign a unique public IP address to each instance.

ExpressRoute failover – High-availability. Configures a VPN gateway as a secure failover path for ExpressRoute connections. Resiliency built in.

Zone-redundant gateways – VPNs and ExpressRoute can be deployed in a zone-redundant configuration. This configuration brings resiliency, scalability, and higher availability to virtual network gateways.

- _ExpressRoute_

Let’s you extend your on-premises networks into the Microsoft cloud over a private connection, with the help of a connectivity provider. You can establish connections to Microsoft cloud services, such as Azure and 365. Allows you to connect offices, datacentres and other facilities to the cloud.

- _Azure DNS_

Hosting service for DNS domains that provides name resolution by using Microsoft Azure infrastructure.

- _Azure storage accounts_

Storage account provides a unique namespace for your Azure storage data that’s accessible anywhere around the world.

Storage account names must be between 3-24 characters in length and contain numbers and lowercase letters only.

No storage accounts can have the same name.

- _Azure storage redundancy_

Redundancy ensures that your storage account meets its availability and durability targets even when failure occurs.

Locally redundant storage – Replicates data three times within a single data centre in the primary region. Lowest cost redundancy.

Zone-redundant storage – For availability zone-enabled regions, zone-redundant storage replicates your Azure storage data synchronously across three Azure availability zones in the primary region.

Redundancy in the secondary region – Data is stored in a secondary region in case of catastrophic failure in primary region.

Geo-redundant storage – Copies your data synchronously three times within a single physical location in the primary region. It then copies your data asynchronously to a single physical location in the secondary region.

Geo-zone-redundant storage – Combines high availability provided by redundancy across availability zones with protection from regional outages by geo-replication.

- _Azure storage services_

Azure Blobs – Massively scalable object store for text and binary data. Also includes support for big data analytics through Data Lake Storage Gen2. Hot – Data used a lot. Cool – Data used infrequently. Cold – Data hardly used. Archived – Data basically never used.

Azure Files – Managed files shares for cloud or on-prem deployments.

Azure Queues – A messaging store for reliable messaging between application components.

Azure Disks – Block-level storage volumes for Azure VMs.

Azure Tables – NoSQL table option for structured, non-relational data.

- _Azure data migration_

Azure Migrate is a service that helps you migrate from on-premises environment to the cloud. Azure Migrate functions as a hub to help you manage the assessment and migration of your on-prem datacentre to Azure.

Azure Migrate: Discovery and assessment: Discover and assess on-prem servers running on VMware, Hyper-V and physical servers in prep for the migration to Azure.

Azure Migrate: Server migration: Migrate VMware VMs, Hyper-V VMs, physical servers, other virtualised servers, and public cloud VMs to Azure.

Data Migration Assistant: Data Migration Assistant is a stand-alone tool to assess SQL servers. It helps pinpoint potential problems blocking migration.

Azure Database Migration Service: Migrate on-prem databases to Azure VMs running SQL server, Azure SL Database, or SQL Managed Instances.

Azure App Service migration assistant: Azure App Service migration assistant is a standalone tool to assess on-prem websites for migration to Azure App service. Use Migration Assistant to migrate .NET and PHP web apps to Azure

Azure Data Box: Use Azure Data Box products to move large amounts of offline data to Azure.

- _Azure file movement options_

AzCopy – CLI utility that you can use to copy blobs or files to or from your storage account.

Azure storage explorer – Standalone app that provides a graphical interface to manage files and blobs in your Azure storage account. It works on Windows, macOS, and Linux operating systems and uses AzCopy on the backed to perform all the file and blob management tasks.

Azure file sync – Tool that lets you centralise your file shares in Azure files and keep the flexibility, performance, and compatibility of a Windows file server, it’s almost like turning your Windows file server into a miniate content delivery network.

- _Azure directory services_

Microsoft Entra ID is a directory service that enables you to sign in and access both Microsoft cloud applications and cloud applications that you develop.

Can also help you maintain your on-premises Active Directory deployment.

Provides authentication, SSO, application management and device management.

Microsoft Entra Domain Services – Service that provides managed domain services such as a domain join, group policy, lightweight directory access protocol, Kerberos/NTLM authentication.

- _Authentication methods_

SSO – User signs in once and has access to all resources without having to sign in again

MFA – Something the user knows, has, is. 2FA.

Microsoft Entra Multifactor authentication – Microsoft service that provides multifactor authentication capabilities.

Password less – Windows Hello for Business, Microsoft Authenticator App, FIDO2 security keys.

- _External identities_

B2B – Business to business collaboration

B2C – Business to customer collaboration

- _Azure conditional access_

Used to allow or deny access to resources based on identity signals. Signals include who the user is, where the user is, and what device the user is requesting access from.

- _Azure role-based access control_

Only have access to your role and nothing else. No excess access privileges are provisioned, only the ones needed to perform your role.

- _Zero-trust_

Verify explicitly, use least privilege access, assume breach.

- _Defence in depth_

Multiple layers of security to reduce attack surface and uses multiple layers to stop attackers.

- _Microsoft Defender for Cloud_

Monitoring tool for security posture management and threat protection.

Protection everywhere you’re deployed.

**Describe Azure management and governance (30–35%):**

- _Azure costs_

CapEx – Building infrastructure

OpEx – Renting infrastructure

OpEx cost can be impacted by – Resource type, consumption, maintenance, geography, subscription type, Azure marketplace.

- _Pricing calculator_

Calculator designed to give you an estimated cost for provisioning resources in Azure.

- _Total cost calculator_

Calculator designed to help you compare the costs for running an on-premises infrastructure compared to an Azure cloud infrastructure (TCO).

- _Microsoft Cost Management tool_

Cost management - Provides the ability to quickly check Azure resource costs, create alerts based on resource spend, and create budgets that can be used to automate management of resources.

- _Tags_

Tags are a way to organise resources.

Tags provide extra information, or metadata, about your resources.

- _Microsoft Purview_

Microsoft Purview is a family of data governance, risk, and compliance solutions that helps you get a single, unified view into your data.

Brings insights about your on-premises, multi-cloud, and SaaS data together.

- _Azure policy_

Azure policy is a service in Azure that enables you to create, assign, and manage policies that control or audit your resources.

User creates policies and Azure policies will check if resources are compliant etc.

Policy initiatives – Way of grouping related policies together.

- _Resource locks_

Prevents resources from being accidentally deleted or changed.

Two types, one that prevents deletion and one that prevents changes from being made.

- _Service Trust Portal_

Portal that provides access to various content, tools, and other resources about Microsoft security, privacy, and compliance practises.

For example, ISO/IEC is there, GDPR, etc.

Can be added to library to stay up to date with regulations and standards.

- _Tools for interacting with Azure_

Azure portal, PowerShell, CLI.

- _Azure Arc_

Utilising Azure Resource manager (ARM), Arc lets you extend your Azure compliance and monitoring to your hybrid and multi-cloud configurations.

Azure Arc simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.

Azure Arc basically lets you manage your entire environment.

- _Azure resource manager (ARM)_

Deployment and management service for Azure.

Provides a management layer that enables you create, update, and delete resources in your Azure account.

Infrastructure as code (IAC) – Concept where you manage your infrastructure as lines of code. Basically, Azure Cloud Shell, Azure PowerShell, or the Azure CLI to manage and configure your resources.

ARM templates – You can describe the resources you want to use in a declarative JSON format. With an ARM template, the deployment code is verified before any code is rum. This ensures that the resources will be created and connected correctly. The template, then orchestrates the creation of those resource in parallel. That is, if you need 50 instances of the same resource, all 50 instances are created at the same time.

Bicep – Language that uses declarative syntax to deploy Azure resources. A Bicep file defines the infrastructure and configuration. Then, ARM deploys that environment based on your Bicep file.

- _Azure Advisor_

Azure Advisor evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs.

Is designed to help you save time on cloud optimisation.

- _Azure Service Health_

Azure Service Health helps you keep track of Azure resource, both your specifically deployed resources and overall status of Azure.

Does this by combining: Azure status, Service health, resource health.

- _Azure Monitor_

Azure Monitor is a platform for collecting data on your resources, analysing that data, visualising the information, and even acting on the results.

Azure Monitor can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.

Azure Log Analytics – Tool in the Azure portal where you’ll write and run log queries on the data gathered by Azure Monitor. Robust tool that supports both simple, complex queries, and data analysis.

Azure Monitor Alerts – Automated way to stay informed when Azure Monitor detects a threshold being crossed. Set the alert conditions, the notification actions, and then Azure Monitor Alerts notifies when an alert is triggered.

Application Insights – Monitors your web applications. Application Insights is capable of monitoring applications that are running in Azure, on-premises, or in a different cloud environment.

**Material from John Savill’s AZ-900 Study Cram:**

Types of cloud:

- Agility – Change what I’m doing as needs change. Usage amount changes. Change quickly.
- Consumption based – Pay for what you use.
- High availability – Distribution of resources across different zones.
- Disaster recovery – Big distance, 100 of miles in case of natural disaster.
- Scalability – Allocate/deallocate resources.
- Public cloud – Externally hosted by a cloud provider. Multi-tenant. Accessed over internet. Consumption-based. Many locations.
- Private cloud – Dedicated exclusively to a single organisation. Enhances security and control. On-prem.
- Hybrid cloud – Mixture of both public and private.

CapEx, OpEx and consumption-based:

- CapEx – Pay for it upfront.
- OpEx – Renting. Pay-as-you-go.

Shared responsibility and types of service:

- On-premises – Customer is responsible for everything.
- IaaS – Customer is responsible up to operating system.
- PaaS – Customer responsible for Apps and Data.
- SaaS – Customer responsible for users and access.

Regions, environments and Availability Zones:

- Regions – Azure has many regions. Multiple physical locations. Sovereignty requirements. Disaster recovery – 100 miles between.

Updates are staggered to ensure availability between regions.

- Availability zones – Resilience when distributing services over multiple buildings. Subscription will allow you to see availability zones.
- Services – Zone redundant (Automatic redundancy). Zonal (Created in a specific availability zone).

Identify, authentication, authorisation and Azure AD:

- Azure AD – Cloud ID Key. Used by Azure. Within there are users, groups, devices, applications.
- Authentication – Proving who a user is. Something I know, have and am. MFA/2FA.
- Authorisation – Level of access I have. What can I do? RBAC.

Conditional access and SSO:

- Conditional access – Based on certain conditions, enforce MFA.
- SSO – User signs on once and has access to all resources. Through AAD Connect.

Governance (RBAC, Policy, Budget):

- RBAC – Scope. Giving a user, group a certain set of permissions at a certain scope.
- Policy – Control where and how you can perform actions. Policy is a guardrail for example.
- Budget – How much I want to control how much you create. Control spending through trends for example.

Scopes (Management groups, subscriptions and resource groups):

- Management groups – Hierarchy of management groups to fit needs. RBAC, Policy, Budget. Inherited.
- Subscriptions – Subscriptions for different purposes.
- Resources – Resources get created in a resource group. Resource groups exist in a subscription. Can apply RBAC, Policy and budget to resource groups. Common lifecycle, things will be created, run and deleted together.

ARM and Management interaction:

- Azure resource manager (ARM) – How I talk to Azure. Management interactions.
- ARM JSON templates – Apply a template to ARM for provisioning. Parallel.
- Cloud Shell – PowerShell and Bash/CLI. PowerShell AZ and AZ CLI (Bash).
- Bicep – Converts into JSON template. Human-friendly template.

Resource locks, tags and blueprints:

- Resource locks – Cannot delete or cannot change.
- Tags – Metadata. Key and a value. Do not get inherited. Labels.
- Blueprints – Define list of artifacts wanted and assign it.

Cloud Adoption Framework:

- Cloud adoption framework – Make a plan, get org ready, introduces cloud. How to get started etc.

Key types of compute resource:

- Virtual machine (VM) – Virtual CPU, memory, storage, network config. Collection of resources.
- SKU – Pick a certain number of resources depending on the work it must do.
- Virtual machine scale set – Pick templates, certain configuration and certain scale or auto-scale.
- Azure dedicated host – Paying for entire capacity to fill up with your own VMs.
- Azure batch – Large scale workloads.
- Containers – Virtualising the software. Deploys software to the application a lot easier.
- Azure Kubernetes Service (AKS) – Management/control plane (managed for me). Nodes can be seen by the customer.
- Azure App Service – Web-focused workload. E.g web-app, API service, mobile app. PaaS.
- Serverless – Don’t pay for VM. You pay for the work it does. Event-driven, something must happen.
- Azure Function – Running code I have written. Short-lived. Little piece of work then goes away.
- Azure Logic Apps – No/low code. Prebuilt connectors can be drag and dropped.
- Azure Virtual Desktop – Publishing a session and/or an application. VMs which are your host.

Azure Key Vault:

- Secrets, keys, certificates held.
- Access policies or RBAC are used to access Azure Key Vault.

Networking:

- Virtual network – Within a subscription and a region.
- Virtual subnets – IP range assigned.
- Peer – Route them over Azure.
- Gateway – VPN, over the internet creates a tunnel for connection. Encryption. Policy – One connection. Route based – Point-site VPN, multiple tunnels used.
- ExpressRoute – Private connection, doesn’t go over the internet, private connection. Private peering.
- Network Security Groups (NSGs) – Segments networks, filtering traffic, allowing and disallowing connections. (Layer 4)
- Service tags – Represents a set of IPs used by a particular service.
- Azure Firewall – Network, application rules (Layer 4/7). User defined routes to Azure Firewall.
- Service endpoint – Better route to service. Only things that exists in the subnet.
- Private endpoint – IP address in the subnet that points to a specific version in the service.
- DDoS protection service – Basic and standard. Basic – Huge scale, redirects traffic. Standard – Create a standard plan and you can link that plan to different VNETs. Standard is more advanced than basic. Standard – ML.

Storage accounts:

- Storage account – Name, lives within a region, redundancy, availability zones.
- Paired-region – 100s of miles away in the same geopolitical boundary.
- Local redundant storage (LRS) – Three copies of the data in the same cluster.
- Zone redundant storage (ZRS) – Three copies of data spanning multiple availability zones.
- Geopolitical redundant storage (GRS) – Three copies of data in one region and three copies in the paired region.
- Geopolitical zone redundant storage (GZRS) - Three copies of data in multiple regions and three copies in the paired region. Read-only available.
- Standard – All options are available.
- Premium – Only has LRS and sometimes ZRS.
- Blob – Binary large object. Block – Blocks. Page – Pages. Append – Logging. Standard one, premium more than one.
- Files – Shares. Azure file sync – Sync on-prem file servers to cloud share.
- Queues – Small messages in a first in, first out format. Event-driven.
- Tables – Key values storage.
- Access tiers – Blob – Hot, cool and archive.
- Lifecycle management – Based on rules I set, can help automate decisions.

Database services:

- SQL – Azure SQL database – Most PaaS solution.
- Azure SQL managed instance – Compatibility when going from on-prem to cloud.
- Migration data service – How I’m using things on-prem, what features I’m using to the integrate to cloud.
- PostgreSQL, MySQL – Open-source options, managed offerings built on open-source.
- Hyperscale – Huge scaling.
- Cosmos DB – Multiple models, documents, SQL, APIs, column-based data, graph can be used. Pick consistency.

Azure Marketplace:

- Place where I can see resources from both Microsoft and third-party options.

IoT Services:

- Azure IoT Hub – All about the ability via SDKs to write App to talk and receive communications.
- Azure IoT Central – Sitting on top of Hub but adding dashboards.
- Azure Sphere – Idea of securing devices.

Data services:

- Azure Data Factory – Orchestration
- Data bricks – Apache Spark. Transformation of data.
- Azure synapse analytics – Orchestration, data warehouse, Apache spark. Brings everything together.

AI services:

- Azure Machine Learning (ML) – Platform for predictions. I’m doing the work on how to get the data, create the models, test the models and deploy the algo.
- Azure Cognitive Services – Pre-built models, based around language, speech, vision, decisions.
- Azure bot service – Interacting with people. Chat bot, voice, knowledge base.

DevOps services:

- DevOps is a process, how people work together etc.
- Repo’s (GIT)
- Boards - Organise and track projects
- Pipelines are continuous integration and delivery. CI/CD.
- Artifacts – Library.
- Test plans.
- GitHub – Repo, actions, CI/CD, projects.
- DevTest Labs – Environments for testing.

Costs in Azure and optimisation:

- Azure Advisor – Gives you guidance on a wide range of areas. Recommendations based on cost.
- Azure Reservations – 1–3-year fixed price discount.
- Hybrid-use benefit – Idea of having license covered and just needing Azure resources.
- Azure spot VMs – Get loaned a VM but can be taken away from a pay-as-you-go customer. Less important work is stored here.

Pricing and TCO calculators:

- Pricing calculator – Estimate the cost of using various Azure services.
- Total cost of ownership calculator – Estimates the cost savings you can achieve by migrating your Workloads to Azure.

Azure Advisor:

- Guidance on cost, performance, resiliency.

Azure Monitor and Service Health:

- Azure Monitor – Metrics go to Azure Monitor
- Diagnostic settings – Log analytics workspace – Log analysis service. Store for up to 2 years. Pay for how long its kept. Event hub – External tool and it can subscribe to the events published (SIEM).
- Service Health – Check health of services from within Azure’s Help tab.

SLAs, status, documents and compliance:

- SLAs – 99.9 % - 10 mins a week it can be down. 99.95% - 5 minutes a week it can be down, 99.99% - 1 minute a week it can be down.
- Azure status – See Azure’s status in every region.
- Compliance – Security, privacy, compliance.
- Trust centre – Rules, regulations and compliance.

Security, Defender for Cloud and Azure Sentinel:

- Defence in depth – Defence in layers. If one failed, another can protect it.
- CIA – Confidentiality, Integrity, Availability.
- Microsoft Defender for Cloud – Hub for security. Secure score to get an overview for how secure you are. Regulatory compliance. JIT.
- Azure Sentinel – SIEM and SOAR. Log analytics workspace. Machine learning.
