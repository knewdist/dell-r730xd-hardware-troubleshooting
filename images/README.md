# Diagnostic Images — Dell PowerEdge R730xd

This directory contains images captured during a real-world hardware incident
involving ECC memory failure on a Dell PowerEdge R730xd.

All images directly support diagnostic conclusions or resolution validation.

---

## Image Index

### 1. UEFI / POST Memory Error
**File:** `UEFI0078.jpg`  
Firmware-level error displayed during POST indicating memory-related faults.

---

### 2. Dell ePSA Memory Diagnostics
**File:** `ePSA.jpg`  
Dell Enhanced Pre-Boot System Assessment showing ECC memory failure.

---

### 3. System Event Log — Memory Error (1)
**File:** `SEL01.jpg`  
System Event Log entry confirming memory-related hardware error.

---

### 4. System Event Log — Memory Error (2)
**File:** `SEL02.jpg`  
Additional SEL entry supporting uncorrectable ECC memory failure.

---

### 5. Failed DIMM Removal (Slot B1)
**File:** `B1-removal.jpg`  
Physical removal of the failed ECC memory module from slot B1.

---

### 6. Proxmox Kernel Memory Verification
**File:** `KERN-MEM.jpg`  
Linux kernel memory output confirming system stability after DIMM removal.

