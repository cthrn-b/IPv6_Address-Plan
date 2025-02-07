# IPv6 Address Plan

## Objective
To design an IPv6 addressing plan for a hypothetical enterprise network, considering efficient allocation, address hierarchy, and future scalability.

## Network Overview
The enterprise consists of the following departments and sub-networks:

- **Headquarters (HQ)** – 300 devices
- **Branch Office 1** – 150 devices
- **Branch Office 2** – 200 devices
- **Data Center** – 500 devices
- **Guest Wi-Fi Network** – 100-500 users (variable)
- **IoT Devices** – 200 devices

## Address Allocation Plan
- **Global IPv6 Prefix**: `2001:db8::/32`
- **Subnet Allocation**:
  - HQ: `2001:db8:1::/48`
  - Branch Office 1: `2001:db8:2::/48`
  - Branch Office 2: `2001:db8:3::/48`
  - Data Center: `2001:db8:4::/48`
  - Guest Wi-Fi: `2001:db8:5::/48`
  - IoT Devices: `2001:db8:6::/48`

## Routing Considerations
- Implement **OSPFv3** for efficient intra-network routing.
- Use **BGP** if external routing to ISPs is required.

## Security Considerations
- **Access Control Lists (ACLs)** to filter traffic between subnets.
- **IPv6 Firewall Rules** for securing critical infrastructure.
- **Monitoring and Logging** for tracking IPv6 traffic.

## Network Diagram
_A network diagram should be included to visualize the allocation of IPv6 subnets._
