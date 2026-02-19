\# Azure Networking Project



\## Overview

This project demonstrates core Azure networking concepts including Virtual Networks (VNets), Subnets, Network Security Groups (NSGs), and VNet Peering.



\## Architecture

\- \*\*vnet-main\*\* (10.0.0.0/16) — Main virtual network

  - snet-web (10.0.1.0/24) — Web tier subnet

  - snet-database (10.0.2.0/24) — Database tier subnet

\- \*\*vnet-secondary\*\* (10.1.0.0/16) — Secondary virtual network

  - snet-app (10.1.1.0/24) — Application subnet



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



\## Load Balancer

\- \*\*lb-web\*\* — Public Load Balancer in UAE North

&nbsp; - Frontend IP: pip-lb-web (Static Public IP)

&nbsp; - Backend pool: backend-pool-web (linked to vnet-main)

&nbsp; - Health probe: probe-http (TCP port 80, every 5 seconds)

&nbsp; - Load balancing rule: rule-http (port 80 → port 80)

