
# Cloud Infrastructure Components Assessment

## 1. Compute Resources

**Purpose:**
Compute resources refer to the processing power and memory capabilities that execute applications and perform calculations. In cloud computing, these are typically virtual machines, containers, or serverless functions that run workloads.

**Importance in Cloud Computing:**
Compute resources are the backbone of cloud services—they process data, run applications, and execute user requests. Without compute resources, no workloads can be deployed or managed in the cloud. They provide the scalability to handle varying workloads, allowing organizations to scale up or down based on demand.

**Relation to the KillerCoda Linux Environment:**
In the KillerCoda environment, I identified the following compute resources:
- CPU Model: Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.0GHz
- Number of CPU Cores: 1 core
- Total RAM: 1.9Gi
- Available RAM: 1.5Gi
- Architecture: x86_64
- Hypervisor: KVM

These compute resources were identified using Linux commands such as `lscpu` and `free -h`, which show the CPU specifications and memory availability of the cloud VM.

---

## 2. Storage Resources

**Purpose:**
Storage resources in cloud computing include persistent and ephemeral data storage solutions such as virtual disks, object storage, and file systems. They hold application data, operating systems, and backups.

**Importance in Cloud Computing:**
Storage is critical for data persistence, disaster recovery, and scalability. Cloud storage allows organizations to store and retrieve massive amounts of data reliably, often with features like automatic replication, versioning, and encryption. It ensures that data remains available even if compute resources are terminated.

**Relation to the KillerCoda Linux Environment:**
In the KillerCoda environment, I identified the following storage resources:
- Total Disk Capacity: 19G
- Used Space: 5.4G
- Available Space: 13G
- Root Partition: /dev/vda1 mounted on /
- Mounted File Systems: /run, /, /dev/shm, /run/lock, /boot, /boot/efi

These storage resources were identified using the `df -h` command, which displays disk space usage and mounted file systems. This represents the persistent storage attached to the cloud VM.

---

## 3. Networking Resources

**Purpose:**
Networking resources in cloud computing manage connectivity, traffic routing, and communication between compute resources, users, and external networks. This includes virtual networks, IP addresses, load balancers, and firewalls.

**Importance in Cloud Computing:**
Networking enables resources to communicate with each other and with the internet. It secures data flow, manages traffic, and ensures high availability and low latency for applications. Networking also provides isolation through Virtual Private Clouds (VPCs) and enables hybrid cloud connectivity.

**Relation to the KillerCoda Linux Environment:**
In the KillerCoda environment, I identified the following networking resources:
- Hostname: ubuntu
- IP Address (Primary): 172.30.1.2
- IP Address (Docker): 172.17.0.1
- Loopback: 127.0.0.1
- Network Interface: enp1s0

These networking resources were identified using commands such as `hostname`, `ip a`, and `hostname -I`. The private IP addresses indicate that this VM is connected to a private cloud network, similar to how cloud VPCs operate.

---

## 4. Operating System

**Purpose:**
The operating system (OS) serves as the foundational software that manages hardware resources, file systems, and provides a platform for applications to run on. In cloud computing, Linux is the dominant OS due to its stability, security, and open-source nature.

**Importance in Cloud Computing:**
An OS abstracts physical hardware and enables virtualization—the core of cloud computing. Without an OS, virtual machines and containers cannot function. Linux, in particular, supports nearly all cloud-native tools and orchestration platforms like Kubernetes, Docker, and Terraform, making it the preferred choice for cloud deployments.

**Relation to the KillerCoda Linux Environment:**
In the KillerCoda environment, I identified the following OS details:
- Operating System: Ubuntu 24.04.4 LTS
- Kernel Version: 6.8.0-138-generic

These OS details were identified using commands such as `cat /etc/os-release` and `uname -r`. Ubuntu is one of the most popular Linux distributions used in cloud environments, and the kernel version is important for ensuring compatibility with cloud applications and drivers.
