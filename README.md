# documentation-cloudcix
Documentation for designing, building and maintaining a CloudCIX Cloud.

CloudCIX is an open source Cloud platform available on the Apache 2.0 licence. Sanitising and uploading of the sourcecode is underway and is expected to be completed by Q2 2020. We welcome community input. Contact developers@cloudcix.com.

#  Deployment Models
*  Open Source Private Cloud
*  Open Source Private Cloud with paid for support is available. Contact sales@cloudcix.com.
    *  design consultancy
    *  installation, configuration and validation
    *  24x7 monitoring
    *  diagnostics and break-fix support
    *  resource utilisation and capacity planning
    *  participation in the CloudCIX RoboSOC automated security system
*  Public Cloud
    *  CloudCIX Limited offers CloudCIX as a multi-region Public Cloud platform
    *  CloudCIX Limited is looking for Data Centre owners interested in operating a CloudCIX region on a franchise basis

#  Deploment Process
![Deployment Process](/static/images/deployment_process.png)

#  Architectural Overview
##  Logical Overview
There are three functional elements to CloudCIX...
*  A provisioning and monitoring (PAM) system manages one or more Clouds. A Cloud can only be managed by one PAM.
*  Each Cloud instance has a central orchestration platform (COP) to implement its UI and API.
*  Each Cloud has one or more Regions that contain the physical hosts used to provide the Cloud services. A software system called Robot provisions the user requested infrastructure.

These functional elements can be represented by this diagram.

![Architectural Overview](/static/images/architectural_overview.png)

##  Pod
A Pod is the unit of physical infrastructure in CloudCIX. A Pod can carry out one or more of the following three functions.
*  Provisioning and Monitoring (PAM)
*  Central Orchestration Platform (COP)
*  Region


