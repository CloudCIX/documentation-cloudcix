#  Build Pod Procedure
A Pod is the fundamental hardware block in CloudCIX. A Pod contains a Juniper SRX firewall, network switches and hosts to carry out the functions of that Pod. There are three possible functions for a Pod.

A Pod can carry out one, two or all three of these functions. The following rules apply to Pods in a CloudCIX
*  Monitoring Pod
    *  Every Pod must be monitored by one and only one Monitoring Pod.
    *  All Pods in a CloudCIX Cloud instance must be monitored by the same Monitoring Pod.
*  Central Orchestration Pod (COP)
*    Each CloudCIX Cloud Instance must have one and only one COP Region
*  Region Pod 
    *  A CloudCIX Cloud instance must have one and only one COP Region.
##  Prerequisites

