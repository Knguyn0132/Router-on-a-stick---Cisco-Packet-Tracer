# Cisco Packet Tracer: Useful `show` Commands

This repository is dedicated to documenting and explaining useful `show` commands for Cisco devices in Packet Tracer. Whether you are a beginner or an experienced network engineer, these commands will help you troubleshoot, verify configurations, and monitor the status of your devices.

## Table of Contents
- [Overview](#overview)
- [Common `show` Commands](#common-show-commands)
  - [`show running-config`](#show-running-config)
  - [`show startup-config`](#show-startup-config)
  - [`show ip interface brief`](#show-ip-interface-brief)
  - [`show vlan brief`](#show-vlan-brief)
  - [`show interfaces`](#show-interfaces)
  - [`show mac address-table`](#show-mac-address-table)
  - [`show spanning-tree`](#show-spanning-tree)
  - [`show version`](#show-version)
  - [`show cdp neighbors`](#show-cdp-neighbors)
  - [`show ip route`](#show-ip-route)
  - [`show interfaces trunk`](#show-interfaces-trunk)
  - [`show ip default-gateway`](#show-ip-default-gateway)
- [How to Use These Commands](#how-to-use-these-commands)
- [Contributing](#contributing)

## Overview
Cisco Packet Tracer is a network simulation tool used for learning and practicing networking concepts. The `show` commands are essential for troubleshooting and verifying the network configuration in Packet Tracer. This guide provides examples and explanations of these commands.

---

## Common `show` Commands

### `show running-config`
**Description:** Displays the current configuration of the device that is stored in RAM.

**Example:**
```
Switch# show running-config
```
**Use Case:** Verify the currently applied settings, including VLANs, interfaces, and routing protocols.

---

### `show startup-config`
**Description:** Displays the configuration stored in NVRAM that the device uses on startup.

**Example:**
```
Switch# show startup-config
```
**Use Case:** Compare the current configuration (`running-config`) with the saved configuration to check for unsaved changes.

---

### `show ip interface brief`
**Description:** Provides a summary of the IP address and status of all interfaces.

**Example:**
```
Router# show ip interface brief
```
**Use Case:** Quickly verify the IP configuration and operational status of interfaces.

---

### `show vlan brief`
**Description:** Displays a summary of VLAN configurations on the switch.

**Example:**
```
Switch# show vlan brief
```
**Use Case:** Confirm VLAN IDs, names, and port assignments.

---

### `show interfaces`
**Description:** Provides detailed information about the status and statistics of all interfaces.

**Example:**
```
Switch# show interfaces
```
**Use Case:** Troubleshoot interface issues, such as errors, drops, or collisions.

---

### `show mac address-table`
**Description:** Displays the MAC address table of the switch.

**Example:**
```
Switch# show mac address-table
```
**Use Case:** Verify the MAC addresses learned on each interface and troubleshoot Layer 2 connectivity.

---

### `show spanning-tree`
**Description:** Displays the Spanning Tree Protocol (STP) status and configuration.

**Example:**
```
Switch# show spanning-tree
```
**Use Case:** Check root bridge election, port roles, and STP topology.

---

### `show version`
**Description:** Provides details about the device's hardware, software, and license.

**Example:**
```
Router# show version
```
**Use Case:** Verify the Cisco IOS version, device model, and system uptime.

---

### `show cdp neighbors`
**Description:** Displays information about directly connected Cisco devices using the Cisco Discovery Protocol (CDP).

**Example:**
```
Router# show cdp neighbors
```
**Use Case:** Identify directly connected devices and their interfaces.

---

### `show ip route`
**Description:** Displays the router's IP routing table, showing connected, static, and dynamic routes.

**Example:**
```
Router# show ip route
```
**Use Case:** Verify the routing table to ensure proper Layer 3 connectivity and routing configurations for router-on-a-stick setups.

---

### `show interfaces trunk`
**Description:** Displays information about trunk interfaces on a switch, including VLANs allowed and the trunking protocol in use.

**Example:**
```
Switch# show interfaces trunk
```
**Use Case:** Verify that trunking is enabled and configured properly for inter-VLAN routing in router-on-a-stick setups.

---

### `show ip default-gateway`
**Description:** Displays the configured default gateway on a switch.

**Example:**
```
Switch# show ip default-gateway
```
**Use Case:** Verify that the correct default gateway is configured for Layer 3 communication from the switch to other network devices.

---

## How to Use These Commands
1. Launch Cisco Packet Tracer and set up your network topology.
2. Open the CLI (Command-Line Interface) for a device (e.g., a router or switch).
3. Type any of the commands listed above to view the corresponding output.
4. Analyze the output to troubleshoot or verify your network configuration.

## Contributing
Contributions are welcome! If you have additional useful `show` commands or suggestions for improving this guide, feel free to open an issue or submit a pull request.



