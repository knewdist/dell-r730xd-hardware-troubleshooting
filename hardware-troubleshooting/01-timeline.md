## Timeline of Events

### T0 — Normal Operation
- Dell PowerEdge R730xd operating normally under Proxmox VE
- OPNsense firewall VM running and routing traffic
- VPN access functional
- External client systems (including Arch Linux workstation) communicating normally through firewall

---

### T1 — Initial Symptoms Observed
- Loss of network connectivity **from the Proxmox host**
- Proxmox web interface intermittently unreachable
- SSH access to Proxmox host failing
- **OPNsense firewall remained accessible**
- VPN tunnel remained active and stable
- Other client devices retained internet access

> This confirmed the issue was isolated to the server, not the firewall or network edge.

---

### T2 — Network Isolation Confirmed
- Arch Linux workstation maintained connectivity to OPNsense
- Firewall UI accessible via LAN and VPN
- No evidence of firewall crash or routing failure
- Physical NIC LEDs on the R730xd observed blinking amber/orange
- Server appeared powered but intermittently unreachable

---

### T3 — Escalation and Console Access
- Complete loss of remote management access to Proxmox host
- Required physical console access
- System reboot initiated for further diagnosis

---

### T4 — BIOS / POST Errors Detected
- UEFI warnings indicating memory configuration changes
- POST messages reporting memory errors
- Errors referenced specific DIMM slots (e.g., B1)
- System halted due to uncorrectable ECC memory errors

---

### T5 — Hardware Diagnostics Executed
- Dell pre-boot hardware diagnostics (ePSA) executed
- Memory tests reported errors consistent with POST messages
- Fault isolated to a specific ECC DIMM module

---

### T6 — Physical Inspection and Intervention
- System powered down and disconnected from input power
- Chassis opened for internal inspection
- DIMMs reseated for verification
- Suspect DIMM removed from the identified slot for isolation testing

---

### T7 — Recovery Attempt
- System powered on with suspect DIMM removed
- Successful boot into Proxmox VE
- No further POST or memory-related errors
- Network connectivity restored
- Proxmox web interface and SSH access stable

---

### T8 — Post-Recovery Verification
- Confirmed OPNsense VM operation
- Verified VPN and routing stability
- Reviewed system logs for additional hardware errors
- Memory capacity reduced, but system stable

---

## Incident Status

- **Root Cause**: Failed ECC memory module
- **Scope**: Isolated to Proxmox host hardware
- **Current State**: Fully operational with reduced memory
- **Remediation Plan**: Replace failed DIMM and revalidate memory configuration

