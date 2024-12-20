# README: Using Show Commands in Cisco Packet Tracer

This README provides instructions on how to use different **show** commands in Cisco Packet Tracer to inspect and verify configurations. These commands are essential for troubleshooting and validating your network setup.

---

## Table of Contents
- [Prerequisites](#prerequisites)
- [Commonly Used Show Commands](#commonly-used-show-commands)
  - [1. Viewing Interface Status](#1-viewing-interface-status)
  - [2. Displaying VLAN Information](#2-displaying-vlan-information)
  - [3. Verifying Trunk Configuration](#3-verifying-trunk-configuration)
  - [4. Checking Routing Table](#4-checking-routing-table)
  - [5. Viewing IP Interface Details](#5-viewing-ip-interface-details)
  - [6. Showing Running Configuration](#6-showing-running-configuration)
- [How to Access the CLI in Packet Tracer](#how-to-access-the-cli-in-packet-tracer)

---

## Prerequisites
1. Install **Cisco Packet Tracer** (version 7.3 or above is recommended).
2. Ensure you have a topology set up with devices such as switches, routers, or PCs.
3. Familiarity with the **Command Line Interface (CLI)** of Cisco devices.

---

## Commonly Used Show Commands
Below are some useful **show** commands categorized by functionality:

### 1. Viewing Interface Status
Use this command to check the status of all interfaces on the device:
```bash
show ip interface brief
```
- Displays:
  - Interface names
  - IP addresses
  - Administrative and operational status (up/down)

### 2. Displaying VLAN Information
To view the VLANs configured on a switch:
```bash
show vlan brief
```
- Displays:
  - VLAN IDs and names
  - Ports assigned to each VLAN

### 3. Verifying Trunk Configuration
To check if an interface is operating as a trunk:
```bash
show interfaces trunk
```
- Displays:
  - Trunking interfaces
  - Allowed VLANs
  - Native VLAN

### 4. Checking Routing Table
On routers, use this command to see the routing table:
```bash
show ip route
```
- Displays:
  - Connected and static routes
  - Routing protocols (e.g., RIP, OSPF, EIGRP)

### 5. Viewing IP Interface Details
To see detailed information about the IP configuration of interfaces:
```bash
show running-config
```
- Displays:
  - IP addresses
  - Subnet masks
  - Interface-specific configurations

### 6. Showing Running Configuration
To view the current configuration on the device:
```bash
show running-config
```
- Displays:
  - All active configurations
  - Interface settings, VLANs, and more

---

## How to Access the CLI in Packet Tracer
1. **Open the Device:**
   - Click on the router, switch, or PC in your topology.

2. **Go to the CLI Tab:**
   - In the device window, select the **CLI** tab.

3. **Enable Privileged Mode:**
   - Type:
     ```bash
     enable
     ```

4. **Run Show Commands:**
   - Enter any of the commands listed above to inspect your configuration.

---

### Example Workflow
If you want to verify VLAN configurations and check trunk ports on a switch:
1. Access the switch's CLI.
2. Type:
   ```bash
   show vlan brief
   ```
3. Then check trunk ports with:
   ```bash
   show interfaces trunk
   ```
4. If issues arise, confirm interface statuses with:
   ```bash
   show ip interface brief
   ```

---

## Troubleshooting Tips
- If a device cannot ping another:
  - Check interface status with `show ip interface brief`.
  - Verify VLAN assignments with `show vlan brief`.
  - Confirm trunking with `show interfaces trunk`.
- Always save your configurations with:
  ```bash
  write memory
  ```

---

Feel free to contribute to this repository by adding more commands or examples!

