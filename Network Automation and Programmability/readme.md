# Automation Goals and Impact
### What is "Network Management"
* Network Management Entails : 
   1. Physical installation of new equipment
   2. Initial configuration of equipment (i.e provisioning)
   3. Monitoring, troubleshooting and testing of equipments
   4. Software upgrades and patches
   5. Configuration Tuning and Enhancements of equipments 
### Methods and Challenges
#### Methods
|For configuring, troubleshooting and software upgrades|Network Monitoring|
|------------------------------------------------------|------------------|
|SSH/Telnet/Console paired with secureCRT|SNMP|
|Notepad|Netflow|
|Scripts||
|SNMP||
#### Challenges
|Challenges| |
|----------|-|
|Large network = large IT staff|requires staff to have knowledge of multiple network OS resulting to Silos of expertise and Huge learning curves|
|Box-by-box management|Easy to make mistakes or lost of documents|
|Knowledge of SNMP configuration and management ||

## Goals of Automation
| | | |
|-|-|-|
|Reduce/eliminate box-by-box management model and eliminate repetitive tasks|Standardise software types and procedures(Golden Image & SOP on upgrades)||
|Apply consistent policy across the network|Reduce time spent on troubleshooting.|Utilisation of scripts and tools to perform mass upgrades/changes|

## What can automated bring about?
| | | |
|-|-|-|
|Plug and play initial provisioning|Path segregation via dynamic overlay networks|Automated dynamic QoS Policies|Automated Topology Visualisations|
|Dynamic Security Policies|Scheduled Software Deployments|Intelligent and automated solutions to troubleshoot problems||

## Automation Origination Points
* Network Management Automation can happen from **3** different origins : 
1. SDN Controllers
2. Server Running Network Management Protocols
3. On-the-box built-in scripts

## Network Management Automation Protocols and Impact
### Common Languages and Protocols
1. Network Monitoring
   - SNMP Managers
   - Netflow Collectors
2. Common Langauges and Protocols
   | | | | |
   |-|-|-|-|
   |CLI carried over SSH|SNMP|NETCONF(XML)/YANG(Yet Another New Gen)|RESTCON(XML/JSON)/YANG|
   |OpenFlow|Cisco OpFlex|REST APIs||

### Impact of Automation
* Cost Reduction
* Time savings and elimination of repitition
* Configuration Consistency
* Elastic scaling
* Network admins will need to become familiar with Server OS, installation, patching and troubleshooting.

# SDN & Automation
## Traditional Networks vs Controller Based Networks
|Traditional Networks|Controller Based Networks|
|--------------------|-------------------------|
|Box-by-Box Management|Dynamic and automatic updates/changes to config based on preconfigured policies|
|CLI-Driven||
|Extensive use of Telnet,SSH,HTTP or SNMP||
|Networking functions implemented in individual devices using vendor proprietary ASICs(Application Specific ICs)|Control Plane functionality to a central SDN Controller|
|Devices start out with minimal or no initial configs|Dynamic implementation of initial configurations (PnP or zero-touch config)|
|Multiple disparate serverse for network management|Controllers consolidate mulitple management services into a box|

### Definition
* Control Plane : 
* Data Plane : 

## 2 Approaches in SDN : 
### Imperative Approach
* Control plane logic resides in the controller
* Controller has complete control over programming the forwarding path of devices.

### Declarative Approach
* Control plane logic resides within the networking devices
* Controller 'declares' the requirements of applications and Network devices decide how to translate that into functional actions.

## Considerations for Including SDN Controller's into Network Design
* Hardware selected must understand the controller's protocol (Most Important!!!)
* Redundant paths to/from controller should exist
* If datacenters are geographically dispersed, one must plan for controller reachability
* Controllers should be configured in clusters for redundancy
* Security as now, router controls are centralised.
* Training for Staff/Team

# DNA Center
# REST
# Network Automation Tools
# Data Encoding and Representation
