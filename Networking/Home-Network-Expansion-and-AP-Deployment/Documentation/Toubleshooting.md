# Troubleshooting

This document outlines the issues encountered during deployment, the troubleshooting process used to identify each problem, and the steps taken to resolve them.

---

# Issue 1: Incorrect WAN Connection Detection

## Symptoms

During the initial setup, the Mercusys router automatically detected the WAN connection type as PPPoE. After completing the setup, the router was unable to establish an internet connection.

## Investigation

The following troubleshooting steps were performed:

- Verified all physical Ethernet connections.
- Confirmed the ISP connection was connected to the WAN port.
- Restarted the router and attempted the setup process again.
- Reviewed the WAN configuration options available on the router.
- Contacted the Internet Service Provider to verify the required WAN configuration.

## Root Cause

The ISP confirmed that the internet service was configured using a **Static IPv4** connection rather than PPPoE authentication.

Because the router automatically selected PPPoE, it attempted to authenticate using a protocol that was not supported by the ISP.

## Resolution

The router's WAN configuration was manually changed to Static IPv4.

The ISP-provided network information was entered manually, including:

- Static IPv4 address
- Subnet mask
- Default gateway
- DNS server information

## Result

The router successfully established internet connectivity after the correct WAN configuration was applied.

---

# Issue 2: Preventing Multiple DHCP Servers

## Potential Issue

Using two routers with DHCP enabled can cause multiple devices to assign IP addresses on the same network.

This may result in:

- IP address conflicts
- Incorrect default gateway assignments
- Connectivity issues
- Inconsistent client network configurations

## Resolution

The TP-Link router was reconfigured as a wireless access point by:

- Disabling its DHCP server
- Assigning a static LAN management IP address
- Connecting it to the primary router using a LAN-to-LAN Ethernet connection

The Mercusys router remained the only DHCP server on the network.

## Result

All client devices received consistent network configuration from a single centralized DHCP server.

---

# Issue 3: Maintaining Access to the Access Point

## Potential Issue

If the TP-Link router continued using DHCP or obtained its address dynamically, locating and managing the device later could become more difficult.

## Resolution

A static LAN IP address outside the DHCP pool was assigned to the TP-Link router.

This ensured the management interface would always remain accessible without conflicting with dynamically assigned client addresses.

## Result

The access point could be managed consistently using its assigned LAN IP address.

---

# Issue 4: Extending Wireless Coverage

## Problem

Wireless signal strength was weaker in the guest room due to the distance from the primary router.

## Resolution

The existing TP-Link router was repurposed as a wireless access point and installed closer to the guest room.

The access point was connected to the primary router using a wired LAN-to-LAN Ethernet connection while remaining part of the same local network.

## Result

Wireless coverage was extended into the target area while maintaining a single subnet, centralized routing, and centralized DHCP management.
