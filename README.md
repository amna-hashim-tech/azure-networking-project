\# Azure Networking Project



\## Overview

This project demonstrates core Azure networking concepts including Virtual Networks (VNets), Subnets, Network Security Groups (NSGs), and VNet Peering.



\## Architecture

\- \*\*vnet-main\*\* (10.0.0.0/16) — Main virtual network

&nbsp; - snet-web (10.0.1.0/24) — Web tier subnet

&nbsp; - snet-database (10.0.2.0/24) — Database tier subnet

\- \*\*vnet-secondary\*\* (10.1.0.0/16) — Secondary virtual network

&nbsp; - snet-app (10.1.1.0/24) — Application subnet



\## VNet Peering

\- peer-main-to-secondary — Connects vnet-main to vnet-secondary

\- peer-secondary-to-main — Connects vnet-secondary to vnet-main

\- Status: Connected \& Fully Synchronized



\## Resources

\- Resource Group: rg-networking-practice

\- Region: UAE North

\- NSG: nsg-web (attached to snet-web)



\## Skills Demonstrated

\- Azure Virtual Network design

\- Subnet planning with CIDR notation

\- Network Security Group configuration

\- VNet Peering setup and verification

\- Azure CLI (PowerShell)

