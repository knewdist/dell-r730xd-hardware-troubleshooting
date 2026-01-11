# Hardware Incident Case Study  
**Dell PowerEdge R730xd — ECC Memory Failure**

This directory documents a real-world hardware incident involving a Dell PowerEdge R730xd running Proxmox VE and an OPNsense firewall VM.

The incident manifested as intermittent loss of connectivity and management access from the Proxmox host, while the firewall and VPN remained operational.

The investigation followed a structured incident response methodology, progressing from scope isolation to firmware diagnostics, hardware testing, and controlled remediation.

---

## Environment

- Server: Dell PowerEdge R730xd
- BIOS: Dell UEFI
- Memory: ECC DDR4
- Hypervisor: Proxmox VE
- Firewall: OPNsense (VM)
- Use Case: Virtualization, firewall, homelab infrastructure

---

## Investigation Flow

1. **Timeline**  
   [01-timeline.md](01-timeline.md)  
   High-level sequence of events and decision points.

2. **Diagnostics**  
   [02-diagnostics.md](02-diagnostics.md)  
   Firmware, vendor, and hardware diagnostics used to isolate the fault.

3. **Root Cause Analysis**  
   [03-root-cause.md](03-root-cause.md)  
   Technical explanation of the underlying failure.

4. **Resolution**  
   [04-resolution.md](04-resolution.md)  
   Corrective actions taken to restore system stability.

5. **Lessons Learned**  
   [05-lessons-learned.md](05-lessons-learned.md)  
   Operational takeaways and process improvements.

---

## Supporting Evidence

Diagnostic screenshots and photos captured during the incident are available in:

- [`/images`](../images)

These images provide firmware-level errors, vendor diagnostics, physical remediation evidence, and OS-level verification.

