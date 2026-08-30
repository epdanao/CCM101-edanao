# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focused on understanding and documenting the infrastructure required for cloud-based services. In this mission, the Linux environment provided through the KillerCoda Playground is investigated to identify its compute, storage, networking, and operating system resources.

The activity simulates the planning stage of a cloud deployment for a fictional company. The collected infrastructure information is documented and related to fundamental cloud computing concepts. The mission also involves researching official documentation from major cloud providers, comparing their infrastructure services, and creating a basic cloud infrastructure blueprint. The completed documentation is organized as part of the GitHub Cloud Computing Portfolio.

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate hardware and software resources available in a Linux cloud environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret how different cloud infrastructure components work together.
- Compare equivalent infrastructure services offered by AWS, Microsoft Azure, and Google Cloud Platform.
- Create a simple cloud infrastructure diagram.
- Produce organized and professional technical documentation using Markdown.
- Continue developing a structured GitHub Cloud Computing Portfolio.
  
## Cloud Infrastructure Components

The main cloud infrastructure components identified were:

- **Compute:** Intel Xeon E312xx (Sandy Bridge, IBRS update) processor with 1 CPU core and approximately 1.9 GiB of RAM.
- **Storage:** A 19 GB main disk (/dev/vda1) used for the root file system, with additional partitions for /boot and /boot/efi.
- **Networking:**  Private IP addresses 172.30.1.2 and 172.17.0.1 used for internal network connectivity.
- **Operating System:** Ubuntu 24.04.4 LTS with Linux kernel version 6.8.0-138-generic, which manages the server's resources and provides the environment for running commands and applications.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux
- GitHub
- Markdown
- Microsoft PowerPoint / Diagramming Tool
- Web Browser

## Linux Commands Executed

The following commands were used to investigate the Linux environment:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h
hostname
hostname -I
```

## Skills Learned

In this laboratory activity, I learned how to investigate a Linux server running in a cloud environment and identify the resources available in the system. I gained a better understanding of how compute, storage, networking, and operating system resources work together in cloud infrastructure. I also learned how to compare equivalent services offered by AWS, Microsoft Azure, and Google Cloud Platform. In addition, I practiced creating a simple cloud infrastructure diagram and organizing technical information using Markdown and GitHub.

## Challenges Encountered

The challenges I encountered included remembering and using the correct Linux commands to collect the required information from the cloud environment. I also found it challenging to interpret some of the system information, particularly the mounted file systems and network addresses. Another challenge was organizing the collected information clearly in Markdown and comparing services from different cloud providers because they use different names for similar infrastructure services. Creating the infrastructure diagram was also challenging because I needed to properly identify and connect the required cloud components.
