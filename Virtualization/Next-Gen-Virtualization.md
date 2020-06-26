# Next-Gen Virtualization

## Index

- [Chapter 1: Considering the Rise of the Digital Economy](#chapter-1-considering-the-rise-of-the-digital-economy)
- [Chapter 2: It All Begins with Virtualization](#chapter-2-it-all-begins-with-virtualization)
- [Chapter 3: Key Characteristics of Next-Gen Virtualization](#chapter-3-key-characteristics-of-next-gen-virtualization)
- [Chapter 4: Going Beyond Server Virtualization](#chapter-4-going-beyond-server-virtualization)
- [Chapter 5: Next-Gen Virtualization Preflight](#chapter-5-next-gen-virtualization-preflight)
- [Chapter 6: Ten Best Practices for Your Next-Gen Virtualization Platform](#chapter-6-ten-best-practices-for-your-next-gen-virtualization-platform)

# Chapter 1: Considering the Rise of the Digital Economy

Modern virtualization platforms are needed for applications that are highly scalable, available, and secure. Every company now needs to become more software-centric to stay relevant and thrive in the digital economy. Hardware may be familiar, but software is the arena where real change is happening.

## Challenges faced by IT

To succeed in this new software-driven world, every company needs to accelerate the development and delivery of the applications and services that keep customers happy and the businesses competitive. The goal is to drive faster delivery of the resources that empower the business. And at this point, things get harder. In many IT shops, the route to a faster, more agile data center is riddled with roadblocks:

1. **Complexity:** Complex IT architectures and processes limit your agility and flexibility, and create barriers to change.
2. **Budget constraints:** Shrinking or static budgets make it difficult for you to meet the business demands with traditional infrastructure models.
3. **Compliance:** Business units are turning to public clouds for on-demand access to IT services, causing operational cloud silos and compliance risks.
4. **Out-dated architecture:** With current architectures, there is no easy way for you to offer services seamlessly and securely across traditional infrastructure, on-premises private clouds, and public clouds.

Challenges like these point to the need for some serious rethinking of IT architectures and processes. In particular, your organization needs to move to an agile, service-oriented model that is based on a flexible software-defined data center (SDDC) that leverages both private and public clouds.

# Chapter 2: It All Begins with Virtualization

This chapter provides a brief primer on virtualization and its evolution in the data center.

## Understanding Virtualization

Virtualization creates a software representation of the underlying hardware and enables you to run multiple virtual machines on top of a single host. Each virtual machine has its own operating system and application running inside. By doing so, virtualization enables much higher levels of utilization and efficiency.

The practice of virtualization began when IT organizations were wrestling with the limitations of x86 servers that were designed to run just one operating system and one application at a time. As a result of this limitation, even small data centers had to deploy many servers, each operating at 5 percent to 15 percent of capacity. By any standards, utilization rates along those lines are not just inefficient; they’re downright wasteful. Virtualization fixes this problem.

As virtualization technologies evolved, data center operators went beyond server virtualization and started also virtualizing storage and network resources.

## Introducing the Hypervisor

A virtual machine (VM) is a tightly isolated software container with an operating system and application inside. Each selfcontained VM is completely independent of other VMs running on the same host. This independence is made possible by a thin layer of software — called a hypervisor — that is installed on a host computer.

The hypervisor abstracts the underlying server resources and enables the hosting of virtual machines. The host and the resources it controls become part of a larger pool of resources that can be shared by VMs. The hypervisor controls how those resources are accessed by the VMs and dynamically allocates computing resources to each VM as needed.

**Hypervisors come in different flavors. Here are two of the most common:**

1. **Type 1 Hypervisor:**
   The Type 1 hypervisor is referred to as the “bare-metal” hypervisor. This means that it runs directly on the physical hardware of the host machine — it doesn’t have to load an underlying Operating System before that. Due to the fact that Type 1 hypervisors have direct access to the underlying hardware (and no other Operating Systems and device drivers to content with) this type of Hypervisor is considered to be the best performing and most efficient for enterprise computing.
   While considered efficient and well performing, these hypervisors are also known to be very secure. This is because the flaws and vulnerabilities that are endemic to Operating Systems are often absent from Type 1, bare metal hypervisors. The underlying OS has been eliminated. Therefore, each Virtual Machine is isolated from the other and that same isolation guards them against malicious activities or threats.

2. **Type 2 Hypervisors:**
   The main difference between Type 1 and Type 2 hypervisors is that Type 2 hypervisors are typically installed on an existing Operating System. This makes it a hosted hypervisor, seeing as it relies on the host machine’s OS to undertake certain operations like managing calls to the CPU, managing network resources, managing memory and storage. This allows for Type 2 hypervisors to support a wide range of hardware.
   Now, while the goal of both types of hypervisors remained the same, the usage of the underlying Operating System introduced a certain amount of latency. This is because, with a Type 2 hypervisor, all activities and the work of each VM had to go through the host OS.

<p align="center">
      <img src="https://github.com/jashan498/bootcamp/blob/master/Hypervisor.png" alt="Types of Hypervisor" height="400" width="700"/>
</p> <br /> 

## Benifits of using hypervisors

1. **Cost savings:** Right out of the gate, IT organizations turn to virtualization to cut costs. The virtualization of resources leads to increased utilization, reduction in numbers of servers (as well as the associated power and cooling requirements), and more efficient use of valuable data center floor space.
2. **Better resource management:** A virtualized environment is more fluid than a traditional hardwired data center. Your IT administrators can rapidly provision and deploy services and reallocate resources on the fly to balance workloads and improve the performance and availability of applications.
3. **Centralized administration:** When infrastructure resources are virtualized, they can all be monitored and managed from a single console.
4. **Resilience & Higher availability:** A modern virtualization platform incorporates built-in features to help ensure the availability and recoverability of virtualized workloads. The goal is to ensure that data is always available and that applications and services are not interrupted when infrastructure fails.

# Chapter 3: Key Characteristics of Next-Gen Virtualization

A next-gen virtualization platform should have following features:

1. **Infrastructure for connected micro-services:** Micro-services are small strings of modular code that are written to run particular processes. The concept of micro-services is built on the need to develop apps faster, be more resilient, and offer a better user experience. Next-gen virtualization enables your software developers to rapidly deliver the infrastructure for connected micro-services, as well as any other workloads that you run in your data center or from a cloud.

**Note:** An important platform capability here is the ability to orchestrate the restart of micro-services, in which some processes may depend on other processes. Orchestrated restart improves the recoverability of applications that run across multiple VMs. This is done by creating dependency chains between VMs via VM-to-VM restart rules. These restart rules enforce the restart order for each VM within the dependency chain, increasing the likelihood that an impacted application will properly recover when VMs are restarted.

2. **Support for containers and containerized workloads:** Today’s scale-out next-gen applications are increasingly built using Linux containers. Containers bundle an application and everything needed to run it, including system tools and libraries, into a neat package — a complete file system, actually — that can move easily from one computing environment to another. You may have heard of Docker; it’s a well-known software containerization platform.

## Key Characteristics A Platform should have:

Read yourself from Page 18-26.

## Enabling Multi-Cloud Environments

A next-gen virtualization platform also needs to support environments that are more complex:

1. **Support for hybrid environments:** A next-gen virtualization platform is designed from the ground up to support hybrid cloud environments. It allows you to run, manage, connect, and secure your applications across multiple private and public clouds and devices — including apps running natively on leading public clouds.
2. **Workload migration — to the cloud and back:** A fully featured virtualization platform allows you to migrate live workloads not just across servers but also across clusters and clouds and over long distances. To handle spikes in demand, you can migrate workloads from your on-premises data center to the public cloud, and then migrate them back into your data center when demand subsides. This same hybrid approach can be used to enable cloud-based backup scenarios. Throughout the migration, the virtual machine retains its network identity and connections, to help ensure a seamless migration process, whether the workload lands in the public cloud, in your on-premises data center, or in a distant data center.
3. **Consistent management:** Virtualization rises to a higher level with the addition of capabilities for simplified, consistent, and centralized operations management across the virtualized data center. To that end, a comprehensive virtualization platform embeds purpose-built management software that helps you improve the performance, availability, and efficiency of your infrastructure and applications.

## Replacing Physical Infrastructure with Code

Developers want to manage and provision computing infrastructure and its configuration through code. They want to write scripts to remove the need for manual configuration of infrastructure. Given the rapid momentum of the ongoing digital transformation, this capability is no longer just a nice-to-have; it’s becoming a requirement. A forward-looking virtualization platform enables this shift to infrastructure as code through support for DevOps (Development/ Operations) processes, automation, APIs, containers, and more.

1. **DevOps:** A next-gen virtualization platform facilitates DevOps processes to accelerate the development, testing, and release of software applications and updates.
2. **Automation and APIs:** In a world where the infrastructure as code model is emerging as a new requirement in fast-moving DevOps environments, a programmable infrastructure layer is now essential. To that end, users now expect modern software products and frameworks to be accompanied by a well-defined and fully accessible set of programmable APIs.
3. **Support for containers:** To further support the needs of developers, a next-gen virtualization platform offers integrated containers. Containers allow developers to write code once and deploy it anywhere in neat packages of micro-services. In addition, containers help increase the efficiency, speed, and flexibility of development processes. The integrated approach — with support for containers built into the virtualization platform — allows IT teams to run both traditional and containerized applications side-by-side on the same infrastructure without the need for additional tooling or training. So, everybody wins. Developers gain the portability, agility, and speed of containers without disrupting existing workflows, while IT teams get the security, isolation, and management of VMs.

# Chapter 4: Going Beyond Server Virtualization

After you’ve adopted a robust, next-gen virtualization platform, you’re ready to take things to a higher level. You have the foundation for virtualized storage, virtualized networking, and a cloud management platform, all of which move you forward on the path to the **software-defined data center (SDDC)**. This chapter introduces **virtualized storage**, **virtualized networking**, and **SDDCs**.

## Virtualized Storage

**Software-defined storage (SDS)** is one of the key building blocks for **hyper-converged infrastructure (HCI)** and the **SDDC**.  SDS abstracts physical storage constructs to enable flexible and precise consumption according to application requirements. This capability is made possible by the hypervisor, which acts as a broker that balances the needs of a virtual machine and the applications it runs.

### Reinventing the storage model

SDS reinvents the storage model by eliminating legacy silos and enabling the true pooling of storage resources. The hypervisor brings to storage the same operational efficiency that server virtualization brings to compute.
To enable this shift, SDS puts the application and its requirements at the top of the IT food chain, enabling storage resources to respond to the dynamic changes in application requirements. Now the application is the boss and the supporting resources are the workers who make sure the boss gets what the boss needs when the boss needs it.
This is a change from the conventional bottom-up hardwarecentric approach. The conventional approach usually requires your storage admins to create static pools of storage resources and then hope for alignment between the application’s needs and the preprovisioned storage services, often leading to wasted resources (because of overprovisioning to provide for future growth).

### How hyper-converged infrastructure works?

HCI collapses compute, storage (including storage networking), and management onto virtualized, industry-standard hardware, enabling a building-block approach to infrastructure with scale-out capabilities. In HCI, all key data center functions run as software on the hypervisor in a tightly integrated software layer.  HCI implements shared storage by pooling the storage resources distributed across multiple server nodes. You essentially end up with a storage-area network (SAN) inside an x86 server system. So, in the simplest terms, HCI extends the server virtualization technology you already know by abstracting and pooling storage attached to the x86 servers, and incorporating them as part of the virtualized environment.
In an HCI environment, compute, storage, and management resources are delivered through an x86 server platform. The server platform runs a hypervisor and pools direct-attached storage devices together from across multiple servers in the cluster to create shared storage, which acts like that provided by traditional SAN or network-attached storage (NAS) devices.

## Virtualized Networking

### How network virtualization works

Network virtualization makes it possible to programmatically create, provision, and manage networks in software, using the underlying physical network as a simple packet-forwarding backplane.

1.  Network and security services in software are distributed to hypervisors and “attached” to individual virtual machines, based on networking and security policies defined for each connected application.
2.  When a VM is moved to another host, its networking and security services move with it.
3.  When new VMs are created to scale an application, the necessary policies are dynamically applied to those VMs as well.

Similar to the way a virtual machine is a software container that presents logical compute services to an application, a virtual network is a software container that presents logical network services  — logical switching, logical routing, logical firewalls, logical load balancing, logical VPNs, and more  — to connected workloads. These network and security services are delivered in software and require only IP packet forwarding from the underlying physical network. The workloads themselves are connected via a software representation of a physical network “wire”. This allows for the entire network to be created in software.
VMware NSX is designed to serve as a network virtualization and security platform for the SDDC. NSX reproduces the entire network model in software. This end-to-end model enables any network topology — from simple to complex multitier networks — to be created and provisioned in seconds.

### Network virtualization vs software-defined networking(SDN)

Though the term software-defined networking means different things to different people, this much is clear: SDN allows software to control the network and its physical devices. SDN is all about software talking to hardware — you can essentially call it a nextgeneration network management solution. Though it centralizes management and allows you to control network switches and routers through software, SDN doesn’t virtualize all networking functions and components.

In other words, SDN doesn’t allow you to run the entire network in software. Hardware remains the driving force for the network. In contrast to SDN, network virtualization completely decouples network resources from the underlying hardware. All networking components and functions are faithfully replicated in software. Virtualization principles are applied to physical network infrastructure to create a flexible pool of transport capacity that can be allocated, used, and repurposed on demand.

With your networking resources decoupled from the physical infrastructure, you basically don’t have to touch the underlying hardware. Virtual machines can move from one logical domain to another without anyone having to reconfigure the network or wire up domain connections. You implement network virtualization in the hypervisor layer on x86 servers rather than on network switches. The physical network serves as a packet-forwarding backplane controlled from a higher level.

## Cloud management platform

Cloud management platforms deliver the management capabilities that allow you to effectively manage the complete life cycle of services delivered in a hybrid IT environment. These capabilities include the following:

1. **Day-one capabilities:** Allow your IT team to rapidly provision a complete services stack that includes application components along with compute, storage, and network infrastructure.
2. **Day-two capabilities:** Give you the ability to fully manage changes to the service stack, including everything from right-sizing to retirement along with the ability to fully address quality-of-service requirements associated with the running service.

## Considering Software-Defined Data Centers(SDDC)

Public cloud services can be a good fit for many applications, but company-owned data centers continue to play a critical role in enterprise IT, especially for those mission-critical applications that require greater control and security. As a result, many organizations are looking to shift to a more agile, service-oriented IT model that leverages both private and public clouds. The SDDC lays the foundation for this hybrid approach to IT.

### SDDC IN A BOX

In an SDDC, compute, storage, and networking services are decoupled from underlying hardware infrastructure and abstracted into logical pools of resources that can be more flexibly provisioned and managed.
“SDDC in a Box” represents the solutions that bring together the key components of a software-defined data center — including virtualized compute, virtualized storage, and virtualized networking and security — into a natively integrated stack. The result is a ready-to-roll enterprise-class cloud infrastructure.

### SDDC as a Service

SDDC as a Service takes things a step further. This approach offers a fully integrated SDDC software stack via a public cloud, such as Amazon Web Services (AWS) and IBM Cloud. Basically, SDDC as a Service takes the fully virtualized cloud foundation from a private cloud and makes it available via a public cloud.
SDDC as a Service can be adopted as part of a hybrid cloud solution, in which a company pairs the capabilities of an on-premises private cloud with those of a public cloud. In these cases, use of a common virtualization platform enables the seamless integration of the private and public cloud environments.
VMware offers SDDC as a Service in partnership with Amazon Web Services. This offering, VMware Cloud on AWS, enables organizations to rapidly deploy AWS cloud-based resources that are enterprise-grade, secure, and operationally consistent with VMware vSphere–based private clouds.

# Chapter 5: Next-Gen Virtualization Preflight

when a virtual environment is firing on all cylinders, it drives down costs and minimizes downtime while increasing productivity. Unfortunately, many businesses undercut those gains before deployment by incurring costs and causing downtime in the earliest stages of the shift from physical to virtual.

## Preparing to Move from Physical to Virtual

### Assembling your team

Before you move your physical server workloads into virtual machines, enlist a cross-discipline team that includes IT admins, application owners, finance personnel, and other stakeholders. Assemble a detailed plan that outlines the full scope of the project and its phases. Work with your finance team members to determine total cost of ownership (**TCO**) and your projected return on investment (**ROI**).

### Using traditional versus virtual storage

Shared storage improves availability and allows hypervisors to leverage capabilities (such as VMware vMotion) to migrate running VMs across hosts for zero-downtime maintenance. Today, there are multiple options for shared storage:

1. **Traditional external storage-area network (SAN) or network-attached storage (NAS) array:** Compared to virtual storage, a SAN or NAS solution can be more expensive and require more technical expertise because it needs specialized hardware and IT staff. For organizations with available capital and larger IT environments, traditional arrays provide deduplication, array-based replication, and unified storage offerings (for example, NFS, iSCSI, Fiber Channel).
2. **Virtual storage:** This option is simpler than SAN and NAS because you don’t need to purchase, configure, or maintain an external hardware array. For businesses that need shared storage but do not need all the features of an enterprise storage solution, a solution such as VMware vSAN can save capital expenses and ongoing management costs.

### Sizing and managing shared storage

When sizing and managing your shared storage, you should

1. Monitor how much space is used on your existing physical volumes, and also the number of I/O operations per second (IOPS) your workloads use. This information can help you choose the right type and size of disks for your new environment.
2. Calculate your storage needs, in both raw capacity and IOPS, on current and future workloads.
3. Take advantage of the storage efficiencies of virtualization. For example, on a traditional physical server, adding or reconfiguring disk drives is difficult, time consuming, constrained by available drive bays, and can sometimes result in downtime or data loss. In a virtual environment, physical storage devices are abstracted — separated — from the virtual machine, so storage capacity can be added without affecting the VM in any way. Virtual disks, by the same token, can be easily expanded without requiring
4. Choose thin or thick provisioning of virtual disks for individual VMs. Thick provisioning allocates all the space for a virtual disk the moment you create it; thin provisioning allocates space as necessary throughout the virtual disk’s life.

### Addressing security and compliance

Just like physical servers, VMs need to have appropriate security and compliance policies in place. Remember the following:

1. If your business must comply with any government regulations, consider any audit rules that apply. For example, will it be acceptable for each workload to share physical networks or virtual switches? Must the data itself be on separate physical storage?
2. As you set up policies and provisioning, keep in mind the challenge of managing sensitive data from different applications.
3. Make sure you have a working management network with all management interfaces of physical hosts, switches, and other data center infrastructure in the environment.
4. You need to balance VM protection with performance by scheduling security scans and other checks for off hours. Also, consider using features built into vSphere, such as VMware vShield Endpoint, which offloads antivirus and antimalware processes. This approach can also lower the risk of antivirus “storms” by centralizing those functions.

### Using Operations Management to Meet Business Objectives

Server virtualization allows physical resources to be shared among many virtual servers, improving resource utilization. But this isn’t just about utilization. It’s also about performance and security. It’s important to make sure your mission-critical applications have the resources they need to perform well while ensuring they meet your company’s compliance and security policies. Here are some things to consider:

1. Define affinity rules for your VMs. For example, you can define host affinity rules to keep VMs together, so a web server VM and its associated app and database VM are kept on the same physical server for high-speed virtual network connectivity. You can also define anti-affinity rules. For example, you can keep multiple database servers on separate hosts so if a physical host fails, other database VMs will keep running.
2. Determine whether your applications must reside on specific hardware for compliance or process reasons.
3. Make sure you determine the recovery time objective (RTO) and recovery point objective (RPO) for each workload. That way, when you’re creating your business continuity and disaster recovery plans, your backup and recovery policies are aligned with your business priorities.

# Chapter 6: Ten Best Practices for Your Next-Gen Virtualization Platform

Nothing fancy, read it yourself Pg 47-54.
