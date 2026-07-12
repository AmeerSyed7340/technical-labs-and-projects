# Testing and Validation

The following tests were performed after completing the network deployment to verify that the new network operated as expected.

---

# Test 1: Internet Connectivity

## Objective

Verify that the Mercusys router successfully established an internet connection using the ISP-provided static IPv4 configuration.

## Expected Result

The router successfully connects to the Internet.

## Outcome

✓ Successful

Internet connectivity was established after configuring the WAN interface with the ISP-provided static IPv4 settings.

---

# Test 2: DHCP Address Assignment

## Objective

Verify that client devices automatically receive valid network configuration from the Mercusys router.

## Expected Result

Clients receive:

- IP address
- Subnet mask
- Default gateway
- DNS server information

through DHCP.

## Outcome

✓ Successful

Client devices automatically received valid network configuration from the Mercusys DHCP server.

---

# Test 3: Access Point Connectivity

## Objective

Verify that devices connected to the TP-Link access point can access both the local network and the Internet.

## Expected Result

Devices connected through the access point should function identically to devices connected directly to the primary router.

## Outcome

✓ Successful

Client devices connected through the TP-Link access point successfully accessed network resources and the Internet.

---

# Test 4: DHCP Conflict Verification

## Objective

Verify that only one DHCP server is operating on the network.

## Expected Result

The Mercusys router should remain the only device assigning IP addresses.

## Outcome

✓ Successful

The TP-Link DHCP server remained disabled, and all client devices received IP configuration from the Mercusys router.

---

# Test 5: Access Point Management

## Objective

Verify that the TP-Link access point remains accessible through its assigned static management IP address.

## Expected Result

The access point management interface should remain reachable without relying on DHCP.

## Outcome

✓ Successful

The access point remained accessible through its assigned LAN IP address.

---

# Test 6: Wireless Coverage

## Objective

Verify that the additional access point improves wireless coverage in the guest room.

## Expected Result

Client devices maintain reliable wireless connectivity in the target area.

## Outcome

✓ Successful

Wireless coverage was successfully extended to the guest room while maintaining a single local subnet and centralized network management.

---

# Deployment Summary

| Test | Status |
|------|--------|
| Internet Connectivity | ✓ Passed |
| DHCP Address Assignment | ✓ Passed |
| Access Point Connectivity | ✓ Passed |
| DHCP Conflict Verification | ✓ Passed |
| Access Point Management | ✓ Passed |
| Wireless Coverage | ✓ Passed |

The deployment successfully met all project objectives. The Mercusys AC1200 operated as the primary router and DHCP server, while the repurposed TP-Link router functioned as a wireless access point, extending wireless coverage without introducing additional routing or DHCP services.
