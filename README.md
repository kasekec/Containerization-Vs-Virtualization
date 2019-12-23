# Containerization Vs Virtualization
For a long time, there has been a buzz about Virtualization but lately a new buzz  has appeared and this new buzz  seems to confuse everyone. So what exactly is containerization and how does is different from Virtualization?

## First, What is Virtualization?

Virtualization is the process of running a virtual instance of a computer system in a layer abstracted from the actual hardware. Most commonly, it refers to running multiple operating systems on a computer system simultaneously.

Applications running on top of a virtualized machine can appear as if they are on their own dedicated machine, where the operating system, libraries, and other programs are unique to the guest virtualized system and unconnected to the host operating system which sits below it.

### What are the Pros?

* **Reduced Hardware Costs:** Applications no longer need their own server because each virtual machine on the physical server now runs them.
* **Faster Server Provisioning and Deployment:** Server virtualization enables system provisioning and deployment within minutes, allowing you to clone an existing virtual machine without the hours and costs normally spent installing a new physical server.
* **Improved Disaster Recovery:** capability to move a virtual machine from one server to another quickly and safely.
* **Increased Productivity:** Having fewer physical servers means there are less of them to maintain and manage.

### What about the Cons?

* **Extra Costs:** Maybe you have to invest in the virtualization software and possibly additional hardware might be required to make the virtualization possible. This depends on your existing network. Many businesses have sufficient capacity to accommodate the virtualization without requiring much cash. If you have an infrastructure that is more than five years old, you have to consider an initial renewal budget.
* **Software Licensing:** This is becoming less of a problem as more software vendors adapt to the increased adoption of virtualization. However, it is important to check with your vendors to understand how they view software use in a virtualized environment.
* **Learn the new Infrastructure:** Implementing and managing a virtualized environment will require IT staff with expertise in virtualization. On the user side, a typical virtual environment will operate similarly to the non-virtual environment. There are some applications that do not adapt well to the virtualized environment.

## What is Containerization then?

Containerization is the encapsulating or packaging up of software code and all its dependencies so that it can run uniformly and consistently on any infrastructure. They are often referred to as “lightweight,” meaning they share the machine’s operating system kernel and do not require the overhead of associating an operating system within each application. Containerization allows developers to create and deploy applications faster and more securely.

### What are the Pros?

* **Portability:** A container creates an executable package of software that is abstracted away from (not tied to or dependent upon) the host operating system, and hence, is portable and able to run uniformly and consistently across any platform or cloud.
* **Speed:** They are “lightweight,” because they share the machine’s operating system (OS) kernel and are not bogged down with extra overhead. This also reduces server and licensing costs while speeding up start-times as there is no operating system to boot.
* **Fault isolation:** Each containerized application is isolated and operates independently of others.
* **Efficiency:** containers are inherently smaller in capacity than a VM and require less start-up time, allowing far more containers to run on the same compute capacity as a single VM. This drives higher server efficiencies, reducing server and licensing costs.
* **Ease of management:** A container orchestration platform automates the installation, scaling, and management of containerized workloads and services.
* **Security:** The isolation of applications as containers inherently prevents the invasion of malicious code from affecting other containers or the host system.

### What about the Cons?

* **Linux-orientated:** Containerisation is generally limited to Linux OSs and applications, as it has evolved from the Linux Containers (LXC) environment. However, Microsoft is working on a container environment for Windows applications, named Drawbridge, which is yet for a release date.
* **Security complications:** Containers introduce some new security challenges. Firstly, the way in which Linux container apps relate to their host machine and it’s OS kernel potentially creates vulnerabilities. Critical kernel subsystems, such as SELinux and Cgroups are not secured by default, but it is possible to secure these. Secondly, the emergence of a growing ecosystem of container template sharing provides cybercriminals with opportunities for distributing malware. Shared containers need to be rigorously screened before usage.
* **OS choice limitations** Since containers share the OS of the host, the OS has to be compatible with the bare metal server to begin with. Hypervisors overcome the major challenge of running legacy or obscure OSs on modern hardware.
* **Unfamiliar development methodology:** Whereas writing applications for VMs, which are in effect the same as physical machines, was a straightforward transition for development teams, containerisation is a new approach to application development and testing. You may need to train or hire new staff to embrace this approach to virtualisation.
* **Container sprawl** Single VMs will often run multiple applications, but containerisation promotes a one-container one-application infrastructure. This means containerisation tends to lead to a higher volume of discreet units to be monitored and managed.

