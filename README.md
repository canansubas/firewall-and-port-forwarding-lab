# Firewall and Port Forwarding Lab – Home Network

## Description
This lab focuses on understanding firewall behavior and port forwarding risks in a controlled home lab environment.

## Environment
- Internet Connection: VDSL (lab only)
- Modem: TP-LINK VC220-G3u
- OS: Kali Linux (VirtualBox NAT)
- Tools: tcpdump, python, nmap

## Objectives
- Understand firewall rule logic
- Configure and test port forwarding
- Analyze security risks of exposed services

## Lab Topology
(Will be added)

## Experiments
- Baseline firewall behavior
- Port forwarding a local HTTP service
- Restricting access using firewall rules

## Security Notes
All experiments were conducted in a legal, isolated lab environment.

## Baseline Observation
- HTTP service is reachable locally
- No inbound access from external networks
- Firewall and NAT prevent unsolicited inbound connections

## What is Port Forwarding?
Port forwarding is a networking technique used to allow external (WAN) traffic
to access a specific service hosted on an internal (LAN) device.
It maps a public-facing port on a router to a private IP address and port.

## Common Use Cases
Port forwarding is commonly used for:
- Hosting web services (HTTP/HTTPS)
- Remote access services (SSH, RDP)
- Game servers
- IP cameras and monitoring systems
- Testing and lab environments

## Advantages and Risks
### Advantages
- Enables access to internal services from the internet
- Useful for testing, development, and self-hosted services
- Helps understand NAT and firewall behavior

### Risks and Disadvantages
- Exposes internal services directly to the internet
- Increases attack surface if services are not secured
- Vulnerable to scanning, brute-force, and exploitation attempts
- Not a security solution by itself