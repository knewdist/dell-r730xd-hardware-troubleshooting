# Hardware Incident Case Study  
**Dell PowerEdge R730xd – ECC Memory Failure**

## Environment
- Server: Dell PowerEdge R730xd
- BIOS Version: 2.19.0
- Memory: 112 GB ECC DDR4 (pre-failure)
- Hypervisor: Proxmox VE
- Firewall: OPNsense (VM)
- RAID Controller: Dell PERC

## Symptoms Observed
- Intermittent NIC disconnects
- OPNsense web GUI inaccessible
- WireGuard VPN instability
- Amber/orange NIC LED activity
- POST failures and UEFI error screens
- CPU Machine Check exceptions

## Impact
- Remote access interruptions
- Firewall and VPN downtime
- Hypervisor instability


## Investigation Flow

1. [Timeline](01-timeline.md)
2. [Diagnostics](02-diagnostics.md)
3. [Root Cause Analysis](03-root-cause.md)
4. [Resolution](04-resolution.md)
5. [Lessons Learned](05-lessons-learned.md)

