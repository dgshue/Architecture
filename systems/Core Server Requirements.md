# gcrNet Server Infrastructure Requirements

This document contains the server roles for the gcrNet infrastructure and requirements. The available budget for the described infrastructure is $49,139.

## Servers Roles

1 x Data Transfer Node ($13,500; Actual: $13,559.19)
1 x General Login Server ($6,500; Actual: $8,456.00)
1 x Network Administration Server (no original budget; Actual: $6,647.33)
1 x IDS Server ($5,750; Actual: TBD)
3 x PerfSonar Servers ($23,389)
- perfSonar Core (Actual: $4,830.62)
- perfSonar JSNN (Actual: $3,487.68)
- perfSonar NC A&T (Actual: TBD)

## Data Transfer Node

The data transfer node provides the high speed data ingress and egress method for the gcrNet using Globus. Attention is paid to maximize throughput for single threaded processes and high-speed networking. The DTN minimum requirements are:

- 3.5Ghz CPU
- 96GB memory
- Support 10Gbps external data transfer
- Support 40Gbps internal data transfer
- 8GB RAID controller cache
- Contain a sperate management port
- Provide at least 30TB of usable storage, idally using tiered storage
- Linux-based OS
- Support IPv6

Addition reference implementations can be found [here](https://fasterdata.es.net/science-dmz/DTN/reference-implementation/). The reference architecture includes the following specifications:

- 2 x Intel Ivy Bridge E5-2643V2 3.5Ghz 6 Core CPUs
- 96GB Memory
- RAID: Adaptec ASR-81605ZQ
- 16 x WD2500BHTZ-0 drives (250GB/ea, 4TB total)
- 40G Mellanox MCX312A-XCBT NIC

Additional considerations include:

- Splitting storage into 2 groups - fast and slow disks - for cost purposes.
- VROC is most likely out of scope
- CPU speed is important - Xeon Gold series is ideal

## General Login Server

The General Login Server is the hub of connecting to the gcrNet. Most often this server will be the first stop for researchers that are accessing systems in the network. Therefore, it should provide the necessary tools to performa basic computation as well as enough storage and resources for non-specialized daily usage. The minimum requirements are:

- Dual 16 core CPUs
- 128GB memory
- Dedicated management port
- 40G+ network connectivity
- OS and Data drive
- 5TB+ data drive

## Network Administration Server 

This server provides the necessary tools for network functionality, including DNS, DHCP, LDAP, and other infrastrcuture services for the gcrNet. The minimum requirements are:

## Intrustion Detection System Server

The IDS provide network security analysis of the external internet link through a mirrored port. Data from the IDS will be used to identify and even act upon network traffic that is identified as a possible threat. The minimum requirements are:

## PerfSonar Servers

The gcrNet consists of 3 perfSonar servers. The core node that provides  measurement for the gcrNet, reporting, and web interface. The two measurement nodes measure performance at the JSNN and NC A&T.

### Measurement Nodes:

### Core Node
