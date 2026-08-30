# Cloud Infrastructure Components

## 1. Compute Resources

#### Purpose
Compute resources provide the processing power required to execute applications, commands, and workloads. The CPU and its available processing cores determine how much processing capability is available to the system.

#### Why It Is Important in Cloud Computing:
Compute resources are important because applications and services require processing power to operate. Cloud computing allows organizations to provision computing resources according to their workload requirements without having to purchase and maintain physical servers.

#### Relation to the KillerCoda:
The KillerCoda server uses an Intel Xeon E312xx (Sandy Bridge, IBRS update) processor and has 1 CPU core available to the environment. The lscpu and nproc commands were used to identify these resources. This demonstrates how a cloud server can provide a virtualized amount of processing capacity to a user.

## 2. Storage Resources

#### Purpose
Storage resources provide space for the operating system, applications, configuration files, logs, and other data. File systems organize this storage and make it accessible to the operating system.

#### Why It Is Important in Cloud Computing:
Storage is important for maintaining data and system files. Cloud environments can provide scalable storage resources so organizations can store information without having to manage physical storage devices themselves.

#### Relation to the KillerCoda:
The main storage resource used in the KillerCoda environment is /dev/vda1, which provides 19 GB of storage for the root file system. The investigation also identified /dev/vda16 mounted at /boot and /dev/vda15 mounted at /boot/efi. The df -h and findmnt commands were used to examine the server's storage and mounted file systems.

## 3. Networking Resources

#### Purpose
Networking resources allow servers and other systems to communicate with one another. These resources include IP addresses, network interfaces, and network configurations.

#### Why It Is Important in Cloud Computing:
Networking enables cloud resources to communicate with users, applications, databases, and other services. Reliable networking is important for accessing cloud applications and connecting different infrastructure components.

#### Relation to the KillerCoda:
The KillerCoda server has the private IP addresses 172.30.1.2 and 172.17.0.1. The hostname -I command was used to identify these addresses. These addresses demonstrate that the cloud environment provides internal network connectivity to the Linux server.

## 4. Operating System

#### Purpose
The operating system manages hardware and software resources and provides the environment in which applications and commands execute. It also manages processes, memory, storage, networking, and system access.

#### Why It Is Important in Cloud Computing:
An operating system provides the foundation on which cloud workloads and services operate. Linux is commonly used for cloud servers because it provides a flexible command-line environment and a wide range of administration and development tools.

#### Relation to the KillerCoda:
The KillerCoda server runs Ubuntu 24.04.4 LTS (Noble Numbat) with Linux kernel version 6.8.0-138-generic. Commands such as cat /etc/os-release and uname -r were used to identify the operating system and kernel. The Linux environment provided the tools needed to investigate the server's compute, storage, and networking resources.
