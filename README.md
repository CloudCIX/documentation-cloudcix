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
    *  CloudCIX Limited are looking for Data Centre owners interested in operating a CloudCIX region on a franchise basis

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

##  SRXPod
The SRXPod is the unit of physical infrastructure in CloudCIX. Networking in CloudCIX is based on the Juniper Networks SRX platform. The Juniper SRX is a Router-Firewall appliance. Each SRXPod has an SRX (or an SRX pair in HA) to implement its security and networking functionality.

