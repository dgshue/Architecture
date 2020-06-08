# gcrNet Core Server Specifications

This document describes the core server specifications of the server infrastructure for the gcrNet. Dell has been selected as the hardware manufacture for the core server infrastructure. The first wave of servers was purchased in April 2020 and includes the:

- Data Transfer Node
- perfSonar - Core
- perfSonar - JSNN
- General Login Server
- Network Admin Server

A second wave is planned that incudes the:

- perfSonar - NC A&T

A thrid wave is planned that includes the:

- Intrustion Detection System

## Data Transfer Node

Dell PowerEdge R740xd 

CPU: 2 x Intel Xeon Gold 5222 3.8Ghz 4 core

Memory: 16 x 8GB 2666MT/s Single Rank RDIMM (128GB)

RAID Controller: Dell PERC H740P, 8GB Cache

Disk:

- OS: 2 x 1.2TB 10K SAS 12Gbps (RAID 1)
- Fast Tier: 4 x 1.92TB SSD 12Gbps (RAID 5)
- Data: 5 x 8TB 7.2k NLSAS 12Gbps (RAID 5)

NIC: 

- Management: Broadcom 57416 10G
- Data: Mellanox TBD

## perfSonar - Core

## perfSonar - JSNN

## General Login Server

Dell PowerEdge R540 

CPU: 2 x Intel Xeon Gold 5218 2.3Ghz 16 core

Memory: 6 x 32GB 2666MT/s Dual Rank RDIMM (192GB)

RAID Controller: Dell PERC H740P, 8GB Cache Low Profile

Disk:

- OS: 2 x 1.2TB 10K SAS 12Gbps (RAID 1)
- Data: 4 x 2.4TB 10K SAS 12Gbps (RAID 5)

NIC: 

- Management: 
- Data: Mellanox TBD Low Profile

## Network Admin Server

Dell PowerEdge R540 

CPU: 2 x Intel Xeon Gold 5218 2.3Ghz 16 core

Memory: 4 x 32GB 2666MT/s Dual Rank RDIMM (128GB)

RAID Controller: Dell PERC H740P, 8GB Cache Low Profile

Disk:

- OS: 4 x 1.2TB 10K SAS 12Gbps (RAID 5)

NIC: 

- Management and Data: Broadcom 57412 Dual Port 10G SFP+ Low Profile