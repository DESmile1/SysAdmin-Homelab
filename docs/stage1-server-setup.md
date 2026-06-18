# Stage 1 — Initial Server Setup

## Overview

Initial Ubuntu server was prepared for infrastructure use and migrated from a default desktop-style configuration to a stable server setup.

---

## Key Changes

- Configured hostname (`srv01`)
- Verified SSH access
- Identified and resolved conflict between NetworkManager and systemd-networkd
- Migrated network backend to systemd-networkd
- Replaced DHCP with static IP configuration
- Configured DNS and default gateway via Netplan

---

## Final State

- OS: Ubuntu 25.10
- Hostname: srv01
- Network backend: systemd-networkd
- IP address: 192.168.88.10
- SSH: operational and stable

---

## Outcome

Configuration files for the network setup can be found in the [configs](https://github.com/DESmile1/SysAdmin-Homelab/tree/main/configs) directory.

Server is now configured as a stable network node suitable for further infrastructure development (hardening, services deployment, automation).
