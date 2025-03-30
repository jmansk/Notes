# Networking Patterns for SMBs

## 1. Flat Network with VLAN Segmentation
- Staff VLAN (10.0.10.0/24)
- Guest VLAN (10.0.20.0/24)
- IoT VLAN (10.0.30.0/24)
- Inter-VLAN routing blocked by default
- Shield provides DHCP, DNS, Firewall for all

## 2. Remote-Only Business
- Hosted Shield with WireGuard
- DNS filtering, VPN-only CA access
- All devices managed via Intune
- Vault hosted remotely or paired with secure share

## 3. Office Hub-and-Spoke
- Office has Shield hardware
- Remote users connect into office
- All traffic passes through Shield (full tunnel)
- Optional: Vault backup from office to offsite Vault

## Usage:
Drop into onboarding documents or client proposals to explain infrastructure plan.
