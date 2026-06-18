# Stage 2 — Secure SSH Access Setup

## Overview

SSH access was extended from basic availability to secure key-based authentication for remote administration from an external client system.

---

## Key Changes

- Generated SSH key pair on client machine (Windows/WSL)
- Deployed public key to server authorized_keys
- Verified SSH key-based authentication workflow
- Validated login without password prompt from client system
- Confirmed correct file permissions for SSH configuration (`~/.ssh`, `authorized_keys`)
- Verified OpenSSH authentication flow using public key cryptography

---

## Final State

- SSH: active and stable
- Authentication method: public key authentication enabled
- Password authentication: still available for fallback
- Client access: Windows/WSL → srv01 established via SSH key
- Server: accepting authorized public key for user `dmitry`

---

## Outcome

Server remote access is now secured using key-based authentication and can be accessed from external systems without password input, ensuring both usability and improved security baseline.
