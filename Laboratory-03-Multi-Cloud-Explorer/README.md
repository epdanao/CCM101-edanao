# Laboratory 03 – Multi-Cloud Explorer

## Linux Server Investigation

I launched an Ubuntu Linux Playground using KillerCoda and used Linux commands to examine the server's operating system, processor, memory, and available storage. The information collected provides a basic understanding of the resources available in the cloud-based Linux environment.

## 1. Operating System

**Command used:**

```bash
cat /etc/os-release
```

**Result:**

* Operating System: Ubuntu 24.04.4 LTS
* Version: 24.04
* Codename: Noble Numbat

The server is running Ubuntu 24.04.4 LTS, a Linux distribution commonly used for server and cloud workloads.

### Screenshot

<img width="774" height="307" alt="killercoda-terminal_1" src="https://github.com/user-attachments/assets/797432be-117f-441d-a121-59ec563b5e1c" />


## 2. CPU Information

**Command used:**

```bash
lscpu
```

**Result:**

* Architecture: x86_64
* CPU Model: Intel Xeon E312xx (Sandy Bridge, IBRS update)
* Number of CPUs: 1
* CPU Frequency: 2.0 GHz
* CPU Cores: 1
* Virtualization: Full
* Hypervisor: KVM

The server is configured with one virtual CPU core using an Intel Xeon E312xx processor. The environment is also running through KVM virtualization.

### Screenshot

<img width="1363" height="401" alt="killercoda-terminal_2 1" src="https://github.com/user-attachments/assets/35cca1c7-678a-4cc3-abb3-5039154a4943" />

<img width="1911" height="793" alt="killercoda-terminal_2" src="https://github.com/user-attachments/assets/b45b1237-1e06-4b53-a3ac-180714574b7b" />

## 3. Memory

**Command used:**

```bash
free -h
```

**Result:**

* Total Memory: 1.9 GiB
* Used Memory: 414 MiB
* Free Memory: 851 MiB
* Available Memory: 1.5 GiB
* Swap: 1.0 GiB

The Linux environment provides approximately 1.9 GiB of RAM, with additional swap space available when required.

### Screenshot

<img width="775" height="87" alt="killercoda-terminal_3" src="https://github.com/user-attachments/assets/1cf51dd9-5c78-4f7c-9779-1e076f7d3f5d" />

## 4. Disk Space

**Command used:**

```bash
df -h
```

**Result:**

* Root Filesystem Size: 19 GiB
* Used Space: 5.4 GiB
* Available Space: 13 GiB
* Usage: 30%

The main filesystem provides 19 GiB of storage, with approximately 13 GiB currently available.

### Screenshot

<img width="472" height="175" alt="killercoda-terminal_4" src="https://github.com/user-attachments/assets/11f90667-d1a2-4c9e-8e37-b1e703a25804" />

# Cloud Migration Options

The Linux server environment could be hosted using virtual machine services from AWS, Microsoft Azure, or Google Cloud. These providers offer cloud infrastructure that can support Linux-based workloads.

| Cloud Provider  | Cloud Service          | Purpose                                                                  |
| --------------- | ---------------------- | ------------------------------------------------------------------------ |
| AWS             | Amazon EC2             | Provides scalable virtual computing capacity for running Linux workloads |
| Microsoft Azure | Azure Virtual Machines | Provides virtual machines for running Linux and other workloads          |
| Google Cloud    | Compute Engine         | Provides virtual machines for applications and cloud workloads           |
