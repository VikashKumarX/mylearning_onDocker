# CONTAINERIZATION VS VIRTUALIZATION
1.Isolation
Virtualization results in a fully isolated OS and VM instance, while containerization isolates the host operating system machine and containers from one another. However, all containers are at risk if an attacker controls the host.
2.Deployment
Virtualization means each virtual machine has its own hypervisor. With containerization, either Docker is used to deploy an individual container, or Kubernetes is used to orchestrate multiple containers across multiple systems.
3.Guest Support
Virtualization allows for a range of operating systems to be used on the same server or machine. On the other hand, containerization is reliant on the host OS, meaning Linux containers cannot be run on Windows and vice-versa.
4.Persistent Virtual Storage
Virtualization assigns a virtual hard disk (VHD) to each individual virtual machine, or a server message block (SMB) if shared storage is used across multiple servers. With containerization, the local hard disk is used for storage per node, with SMB for shared storage across multiple nodes.
5.Load Balancing
Virtualization means failover clusters are used to run VMs with load balancing support. Since containerization uses orchestration via Docker or Kubernetes to start and stop containers, it maximizes resource utilization. However, decommissioning for load balancing with containerization occurs when limits on available resources are reached.
6.Networking
Virtualization uses virtual network adaptors (VNA) to facilitate networking, running through a master network interface card (NIC). With containerization, the VNA is split into multiple isolated views for lightweight network virtualization.
# ABOUT CONTAINER ORCHESTRATION
Container orchestration is the automation of much of the operational effort required to run containerized workloads and services. This includes a wide range of things software teams need to manage a container's lifecycle, including provisioning, deployment, scaling (up and down), networking, load balancing and more.
# ABOUT DOCKER
It is a software development platform for virtualization with multiple Operating systems running on the same host. It helps to separate infrastructure and applications in order to deliver software quickly. It uses Client-Server architecture, which involves the 3 main components that are Docker Client, Docker Host, and Docker Registry. The Docker client communicates with the Docker daemon, which takes care of the building, running, and distributing the Docker containers. The Docker client and daemon can run on the same system or connect a client to a remote Docker daemon. They communicate using REST APIs, over UNIX sockets or a network interface.
