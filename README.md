# Dell PowerEdge R730xd — Hardware Troubleshooting Case Study

This repository documents a real-world hardware incident involving a
Dell PowerEdge R730xd running Proxmox VE and an OPNsense firewall VM.

The system experienced intermittent loss of connectivity from the Proxmox host,
while the firewall and VPN remained operational. The root cause was traced to
a failed ECC memory module producing uncorrectable errors.

This case study demonstrates:
- Host vs network fault isolation
- Use of firmware and vendor diagnostics (UEFI, ePSA, SEL)
- ECC memory failure analysis
- Controlled remediation and validation
- Professional incident documentation

---

## Case Study Documentation

Detailed investigation and resolution steps are available here:

📁 **Hardware Incident Report**  
[`hardware-troubleshooting/`](hardware-troubleshooting)

This includes:
- Timeline of events
- Diagnostics performed
- Root cause analysis
- Resolution steps
- Lessons learned
- Supporting screenshots

