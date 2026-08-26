# Infrastructure Report: Cloud Server Investigation

## Server Information

| Category | Details |
|----------|---------|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel Version | 6.8.0-138-generic |
| Architecture | x86_64 |
| Hypervisor | KVM |

---

## Compute Resources

| Resource | Specification |
|----------|---------------|
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.0GHz |
| Number of CPU Cores | 1 core |
| Total RAM | 1.9Gi |
| Available RAM | 1.5Gi |

---

## Storage Resources

| Resource | Specification |
|----------|---------------|
| Total Disk Capacity | 19G |
| Used Space | 5.4G |
| Available Space | 13G |
| Root Partition | /dev/vda1 mounted on / |
| Mounted File Systems | /run, /, /dev/shm, /run/lock, /boot, /boot/efi |

---

## Networking Resources

| Resource | Specification |
|----------|---------------|
| Hostname | ubuntu |
| Primary IP Address | 172.30.1.2 |
| Docker IP Address | 172.17.0.1 |
| Loopback | 127.0.0.1 |
| Network Interface | enp1s0 |

---

## Commands Used for Investigation

| Command | Purpose |
|---------|---------|
| `cat /etc/os-release` | Display operating system details |
| `uname -r` | Show kernel version |
| `lscpu` | Show CPU architecture and specifications |
| `free -h` | Show memory usage |
| `df -h` | Show disk space usage |
| `hostname` | Show hostname |
| `hostname -I` | Show IP addresses |
| `ip a` | Show network interfaces |

---

## Screenshots

The following screenshots were captured during the investigation:

- `screenshots/server-information.png`
- `screenshots/network-information.png`
- `screenshots/storage-information.png`
