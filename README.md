# zabbix_template_RapidRecoveryCore
A Zabbix Template for RapidRecovery Cores.


## Description
The purpose of this template is to provide basic insights into the status of a **Quest Rapid Recovery** core in your system. 

## Goals
  - General Repository Health Info
  - Protected Agents
   - How many Recovery Points
   - Last protection time
   - State & Status of Replication
   
### Method
By utilizing the standard Quest .MIB file that is included with RR instances, we will use SNMPv1 to query date from the server. Use the standard `{$SNMP_COMMUNITY}` for authentication to the device.

NOTE: By default, SNMP handling on RapidRecovery Cores is disabled. This must be enabled, and ports *<sub>(Default UDP/8161)</sub>* opened on the firewall.
