# System Baseline Report

## Mission Overview

This report presents the initial health check of the Linux server using native command-line tools. The purpose is to check the server's memory, disk storage, CPU load, and running processes before deploying a web application.

## 1. Memory (RAM) Check

The `free -h` command was used to check the server's memory usage.

* **Total RAM:** 1.9 GiB
* **Used RAM:** 409 MiB
* **Free RAM:** 1.2 GiB
* **Available RAM:** 1.5 GiB

The server has approximately 1.5 GiB of available memory during the initial check.

## 2. Disk Storage Check

The `df -h /` command was used to check the storage capacity of the root filesystem.

* **Total Storage:** 19 GB
* **Used Storage:** 5.5 GB
* **Available Storage:** 13 GB
* **Disk Usage:** 30%

Checking disk space before a massive traffic surge is important because the server needs enough storage for application files, logs, temporary files, and other data to prevent storage-related problems.

## 3. CPU and Running Processes

The `top` command was used to observe CPU utilization, system load, memory usage, and active processes.

* **CPU Load Average:** 0.00, 0.00, 0.00
* **Total Tasks:** 126
* **Running Tasks:** 2
* **Total Memory:** 1903.2 MiB
* **Available Memory:** 1495.4 MiB
* **Swap Used:** 0.0 MiB

The server showed a low system load during the observation period. It also had available memory and no swap usage at the time of the screenshot. These results serve as the baseline for comparing resource usage after deploying the web server.

## 4. Screenshots

The following screenshots provide evidence of the host system baseline checks:

* `memory-check.png` — Output of the `free -h` command.
* `disk-check.png` — Output of the `df -h /` command.
* `top-check.png` — Output of the `top` command showing CPU load and running processes.
