# Continue Your Linux Investigation

Linux commands were used in the KillerCoda Playground to check the basic information of the server. The commands were used to find out what operating system it has, what CPU it uses, how much memory is available, and how much disk space it has.

### Linux Commands Used

These are the commands I used during the investigation:

* `cat /etc/os-release` – used to check the operating system and its version.
* `lscpu` – used to check the CPU information of the server.
* `free -h` – used to check the available and used memory.
* `df -h` – used to check the available and used disk space.

### System Information

After running the commands, I found that the server is using **Ubuntu 24.04.4 LTS** as its operating system. It has an **x86_64 architecture** and uses an **Intel Xeon E312xx processor** with 1 CPU.

The server has **1.9 GiB of total memory**. At the time I checked it, around **409 MiB was being used**, while **870 MiB was free**. The main disk has **19 GB of total space**, with **5.4 GB used** and around **13 GB available**.

### Purpose of the Investigation

The purpose of this activity was to learn how to check the basic resources of a Linux server using commands. Instead of using a graphical interface, I was able to get the system information directly from the terminal.

Knowing these details is also useful when moving a server to the cloud. The CPU, memory, and storage information can help in choosing a suitable cloud virtual machine.

### Terminal Output

<img width="451" height="836" alt="image" src="https://github.com/user-attachments/assets/eda9ba20-5124-469f-b706-25be7f5be043" />


### Cloud Migration Recommendation

If this Linux server were moved to the cloud, it could be hosted using a virtual machine service from AWS, Azure, or Google Cloud. These cloud platforms allow users to run Linux servers without having to maintain their own physical server.

* **AWS – Amazon EC2:** EC2 can be used to run a Linux server in AWS. The CPU, memory, and storage of the current server can be used as a guide when choosing an EC2 instance.
* **Google Cloud – Compute Engine:** Compute Engine can be used to create and run a Linux virtual machine in Google Cloud. The resources can be adjusted depending on what the server needs.
* **Microsoft Azure – Azure Virtual Machines:** Azure Virtual Machines can also be used to run a Linux server in Azure. Users can choose the needed CPU, memory, and storage for the virtual machine.

### Recommended Cloud Service

I would choose **Amazon EC2** for this Linux server because it can run Linux-based virtual machines and offers different instance options. The resources can also be adjusted depending on the needs of the server.

Google Compute Engine and Azure Virtual Machines can also be used for the same purpose. The final choice can depend on the cost, performance, and other requirements of the organization.

### Migration Considerations

Before moving the server to the cloud, it is important to check the applications, storage, network settings, and security requirements of the server. The current CPU, memory, and disk information can also help in choosing the right virtual machine.

The organization should also consider the cost of using the cloud, data transfer, security, and monitoring. Planning these things first can help avoid problems during the migration.

### Summary

Based on the investigation, the Linux server is running **Ubuntu 24.04.4 LTS** with an **Intel Xeon E312xx processor, 1.9 GiB of memory, and 19 GB of main disk space**. The server can be moved to AWS through Amazon EC2, Google Cloud through Compute Engine, or Microsoft Azure through Azure Virtual Machines. These services can provide a suitable environment for running the Linux server in the cloud.

