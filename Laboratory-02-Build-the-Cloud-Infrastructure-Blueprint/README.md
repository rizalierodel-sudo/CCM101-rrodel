# Laboratory 02: Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focuses on understanding the fundamental components of cloud infrastructure. As a cloud engineer, I investigated a Linux environment in KillerCoda to identify compute, storage, networking, and operating system resources. This activity simulates the planning phase of a cloud deployment, where documentation and justification of design decisions are essential before any servers are deployed. The goal is to prepare a Cloud Infrastructure Assessment Report that will help senior engineers design the final cloud architecture.

## Objectives

By completing this laboratory activity, I was able to:

- Explain the major components of cloud infrastructure
- Investigate the hardware and software resources available in a Linux environment
- Differentiate compute, storage, networking, and identity resources
- Interpret the relationship between cloud infrastructure components
- Create professional technical documentation using Markdown
- Continue building a structured GitHub Cloud Computing Portfolio

## Cloud Infrastructure Components

Through this laboratory activity, I identified and documented the following cloud infrastructure components:

| Component | Description | Example from KillerCoda |
|-----------|-------------|------------------------|
| **Compute Resources** | Processing power and memory that execute applications | Intel Xeon E312xx @ 2.0GHz, 1 core, 1.9Gi RAM |
| **Storage Resources** | Persistent and ephemeral data storage | 19G disk capacity, /dev/vda1 mounted on / |
| **Networking Resources** | Connectivity and communication between resources | Hostname: ubuntu, IP: 172.30.1.2 |
| **Operating System** | Software that manages hardware and provides a platform | Ubuntu 24.04.4 LTS, Kernel 6.8.0-138-generic |

## Tools Used

| Tool | Purpose |
|------|---------|
| **KillerCoda Playground** | Linux environment for investigating cloud infrastructure |
| **GitHub** | Repository for storing documentation and code |
| **Canva** | Creating the cloud architecture diagram |
| **Linux Command Line** | Running commands to inspect system resources |

## Linux Commands Executed

| Command | Purpose |
|---------|---------|
| `cat /etc/os-release` | Display operating system distribution details |
| `uname -r` | Show the kernel version |
| `lscpu` | Display CPU architecture and specifications |
| `free -h` | Show memory usage in human-readable format |
| `df -h` | Display disk space usage and mounted file systems |
| `hostname` | Show the server's hostname |
| `hostname -I` | Display all IP addresses |
| `ip a` | Show network interfaces and IP addresses |
| `lsblk` | List block devices (disks and partitions) |

## Skills Learned

- Identifying cloud infrastructure components (compute, storage, networking, OS)
- Using Linux commands to inspect system resources
- Creating professional technical documentation using Markdown
- Designing a simple cloud architecture diagram using Canva
- Comparing cloud services across AWS, Azure, and GCP
- Maintaining a structured GitHub portfolio with proper commits

## Challenges Encountered

| Challenge | Solution |
|-----------|----------|
| Understanding the difference between infrastructure components | Reviewed concepts from Chapter 2 and related them to actual system outputs from KillerCoda |
| Interpreting Linux command outputs | Used `man` pages and online resources to understand command options and outputs |
| Creating a clear cloud architecture diagram | Used Canva with a simple vertical layout: Internet → VPC → Database → Server → User |
| Comparing cloud providers | Researched official documentation of AWS, Azure, and GCP and created a comparison table |

---

