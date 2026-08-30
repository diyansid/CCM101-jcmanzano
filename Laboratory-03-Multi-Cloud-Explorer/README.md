# Laboratory 03 – Multi-Cloud Explorer

## Mission Overview

This laboratory activity explores three major public cloud platforms: Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). The activity focuses on researching their services, comparing their capabilities, and recommending suitable cloud platforms for different business requirements.

## Mission Objectives

- Explore AWS, Microsoft Azure, and Google Cloud Platform.
- Identify core cloud services offered by each provider.
- Compare services across cloud platforms.
- Analyze business requirements and recommend suitable cloud solutions.
- Develop technical documentation using Markdown.
- Continue building a professional GitHub Cloud Computing portfolio.

## Cloud Platforms

The three cloud platforms investigated in this laboratory are:

- Amazon Web Services (AWS)
- Microsoft Azure
- Google Cloud Platform (GCP)

## Linux Investigation

A KillerCoda Linux environment will also be investigated to identify its operating system, CPU, memory, and disk information. The results will be used to identify possible cloud services that could host the Linux server.

## Conclusion

This laboratory develops practical skills in cloud platform evaluation, technical research, service comparison, and cloud solution recommendation.

## KillerCoda Linux Server Investigation

The Linux environment was investigated using terminal commands in KillerCoda. The following system specifications were identified:

| System Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS (Noble Numbat) |
| CPU | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Count | 1 |
| Architecture | x86_64 |
| Memory | 1.9 GiB |
| Disk Space | 19 GB total, 13 GB available |

### Equivalent Cloud Services

This Linux server could be hosted using virtual machine services from any of the three major cloud providers:

- **AWS:** Amazon EC2 could be used to create and run an Ubuntu Linux virtual machine with configurable CPU, memory, storage, and networking resources.
- **Microsoft Azure:** Azure Virtual Machines could host an Ubuntu Linux server and allow its computing and storage resources to be configured according to the workload.
- **Google Cloud Platform:** Compute Engine could provide an Ubuntu Linux virtual machine with customizable CPU, memory, disk, and networking resources.

These services provide similar Infrastructure as a Service (IaaS) capabilities, allowing a Linux server to run on cloud infrastructure instead of requiring a locally maintained physical server.

### Commands Used

- `cat /etc/os-release`
- `lscpu`
- `free -h`
- `df -h /`

### Screenshot Evidence

A screenshot of the KillerCoda terminal showing the Linux server investigation is stored in the `screenshots` folder as `killercoda-terminal.png`.

