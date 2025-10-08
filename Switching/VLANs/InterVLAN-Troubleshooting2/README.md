# VLAN Interconnection Troubleshooting Lab

## 🧠 Objective
Fix connectivity issues preventing PC1 from reaching other PCs across VLAN 13 and VLAN 24.

## 🧰 Topology Overview
- **Router (R1)** → Performs inter-VLAN routing (Router-on-a-Stick)
- **Switches** → SW1 (core), SV (access)
- **PCs** → 4 clients across 2 VLANs
  - VLAN 13: 10.0.0.0/25
  - VLAN 24: 10.0.0.128/25

## ⚙️ Identified Problems
1. Misconfiguration on router subinterface `Gig0/0.13`
2. Trunk misconfiguration between SW1 and SV
3. Incorrect default gateways on PCs

## 🛠️ Fix Summary
- Reconfigured router subinterface:
