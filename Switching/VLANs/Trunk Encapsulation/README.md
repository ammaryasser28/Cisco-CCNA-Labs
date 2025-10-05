# VLAN & Trunk Setup (Layer 3 Switch)

- PC1 → VLAN 1  
- PC2, PC3 → VLAN 2  
- Trunk between SW1 and SW2 (Fa0/1)

Use:  
`switchport trunk encapsulation dot1q`  
before `switchport mode trunk`

✅ PC2 ↔ PC3 ping works  
❌ PC1 ↔ PC2 / PC3 no ping
