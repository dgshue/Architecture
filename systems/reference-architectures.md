# gcrNet Systems Reference Architectures

Multiple reference architectures were reviewed in the design of the gcrNet systems. While this information was helpful, much of it was outdated or difficult in sizing equipment for a WAN link of 10G and LAN speed of 40G/100G. 

## DTN Server

[reference architecture](https://fasterdata.es.net/science-dmz/DTN/reference-implementation/)

* SuperMicro SuperStorage 6049P-E1CR24H Server - 24 3.5 inch drive bays
* 2 Intel Gold 6254 CPUs
* 128gb of memory
* Intel VROC HW Key
* Mirrored M.2 boot drives
* 10 6TB 7.2 RPM drives
* Mellanox MCX516A-CCAT Network Adapter
* 3 years of support

## PerfSonar

[reference architecture](https://docs.perfsonar.net/install_hardware_details.html)

* 3 x Dell R640
* Intel Xeon Silver 4112 CPU
* 16gb of memory
* Dell BOSS Boot, 2 x M.2 - 240GB
* 1 x 300gb 15k 3.5 SAS drive
* 3 years of support
* Broadcom 57416 10gb optical network adapter

## Intrusion Detection Server (IDS)/Application Server/Login Server

* Dell R540 
* 2 x Intel Xeon Silver 
* 96gb of memory
* Dell BOSS boot, 2 x M.2 - 240gb
* 4 x 1TB 7.2k NLSAS drives
* Broadcom 57416 10gb optical network adapter
