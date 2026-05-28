# Administration Lab (Arch Linux + QEMU)

---

Practical Linux administration and troubleshooting lab built on Arch Linux running inside QEMU virtualization.

The goal of this project is to build hands-on experience with:
- Linux system administration
- virtualization
- networking
- SSH remote access
- systemd services
- web server management
- monitoring and troubleshooting

This environment was configured manually from a minimal Arch Linux installation.

---

# Technologies Used

- Arch Linux
- QEMU
- systemd
- OpenSSH
- nginx
- Bash
- Linux networking tools

---

# Project Scope

## Virtualization

- Created a virtual machine using QEMU
- Configured virtual disk image (`qcow2`)
- Managed boot order and installation media
- Worked with virtualized networking

---

## Linux Installation & Configuration

- Installed Arch Linux manually
- Configured:
  - hostname
  - users
  - sudo access
  - networking
  - bootloader
  - system services
- Learned Linux boot process fundamentals

---

## Networking

Worked with:
- localhost / loopback
- private IP addressing
- NAT networking
- QEMU port forwarding
- SSH connectivity

Example concepts explored:
- difference between host and VM networking
- why NAT blocks inbound connections by default
- forwarding host ports to guest services

---

# SSH Remote Administration

Configured OpenSSH server and remote access to the VM.

Implemented:
- SSH daemon management with systemd
- remote login from host machine
- SSH host fingerprint verification
- port forwarding for VM access

Example SSH workflow:

```bash
ssh lida@localhost -p 2222
```
This transformed the VM into a remotely administered Linux server environment.

# systemd Service Management

## Managed Linux services using systemd:

- sshd
- nginx
- custom monitoring service

## Worked with:

- service lifecycle
- enable/start/stop/restart
- autostart configuration
- daemon management
- restart policies
- journal logs

## Example commands:

- systemctl status nginx
- systemctl restart nginx
- journalctl -u nginx
- nginx Web Server

Installed and configured nginx web server.

## Tasks completed:

- service setup
- HTTP response testing
- listening port verification
- custom index page deployment
- local connectivity testing

## Example verification:

- curl localhost
- Bash Automation

## Created custom Bash monitoring scripts for:

- uptime checks
- memory usage
- disk usage
- CPU-heavy process inspection
- service status monitoring

## Example tools used:

- uptime
- free
- df
- ps
- systemctl

# Custom Monitoring Service

## Built a custom monitoring daemon using:

- Bash scripting
- infinite monitoring loop
- log generation
- systemd service integration

## Features:

- automatic startup
- restart on failure
- periodic system health logging

## Example monitored data:

- uptime
- RAM usage
- disk usage
- nginx status
- sshd status
Troubleshooting & Diagnostics

## Practical troubleshooting performed during the project:

- SSH service not enabled
- QEMU disk lock conflicts
- booting back into installation ISO
- VM networking limitations caused by NAT
- service verification using ss, systemctl, and journalctl
- debugging failed or inactive services
- analyzing nginx warnings and logs

## Tools used:

- journalctl
- systemctl
- ss
- ps
- tail
- curl
  
## Key Concepts Learned
- Linux service management
- remote administration
- daemon processes
- system logging
- networking fundamentals
- process inspection
- Linux filesystem structure
- operational troubleshooting
- Bash automation
- infrastructure mindset

# Current Status

## Implemented:

- QEMU virtual machine
- Arch Linux installation
- SSH remote access
- nginx web server
- custom systemd services
- monitoring scripts
- logging and diagnostics

## Planned next steps:

- Docker
- reverse proxy configuration
- Grafana & Prometheus
- advanced monitoring
- backup automation
- firewall configuration
- infrastructure automation


