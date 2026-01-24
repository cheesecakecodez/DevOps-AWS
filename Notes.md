# Notes

From task 1.

What is EC2 in AWS?

Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. 

Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster.

You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. 

You can add capacity (scale up) to handle compute-heavy tasks, such as monthly or yearly processes, or spikes in website traffic. When usage decreases, you can reduce capacity (scale down) again.

An EC2 instance is a virtual server in the AWS Cloud. When you launch an EC2 instance, the instance type that you specify determines the hardware available to your instance. Each instance type offers a different balance of compute, memory, network, and storage resources.

What is a virtual Server?

A virtual server is a
 software-based, isolated environment that acts like a physical server, 
running its own OS and applications but sharing the resources (CPU, 
memory, storage) of a single, powerful physical machine using 
virtualization software called a hypervisor. This
 technology efficiently divides one physical server into multiple 
virtual ones, offering cost savings, flexibility, and easier scaling for
 tasks like web hosting, development, and remote access. 

How it works

[**Physical Server](https://www.google.com/search?client=firefox-b-e&hs=NCYU&sca_esv=09a4dc9e07e27686&channel=entpr&sxsrf=ANbL-n6ilUm4Jg8YC_N8gITSG-7xrrRrug%3A1769170062510&q=Physical+Server&sa=X&ved=2ahUKEwiN3v2I0KGSAxWhT2wGHfTbGWkQxccNegUIgAEQAQ&mstk=AUtExfAk1JKM_VpS593TufDrmGKalJR3N_3OfGDmlsAsTfGTQqcji5uTkJfzVzLmdYv7td0o7rqqMTexH1Vv_rNyja5xLUZOIazKM0DLTzbTjKlw_WYO1xvK1ICBkZ-MQ5ZnGUOjoVbKHGs1n2fwW1TccX1N39fIzfsMJWz_GI2EqOoSOF9C-Z7gOif0ReKfh_8nJBPMnEeuLtpCk6-lRUkxQui8wn6oZqFmNT8_dReiGZBzLLERfTdqz2KUnE96C8vSVD7wVXXHnxoh2wYLlRYXqdx1&csui=3) (Host):** The actual hardware (computer) that provides the raw power.

[**Hypervisor](https://www.google.com/search?client=firefox-b-e&hs=NCYU&sca_esv=09a4dc9e07e27686&channel=entpr&sxsrf=ANbL-n6ilUm4Jg8YC_N8gITSG-7xrrRrug%3A1769170062510&q=Hypervisor&sa=X&ved=2ahUKEwiN3v2I0KGSAxWhT2wGHfTbGWkQxccNegUIgwEQAQ&mstk=AUtExfAk1JKM_VpS593TufDrmGKalJR3N_3OfGDmlsAsTfGTQqcji5uTkJfzVzLmdYv7td0o7rqqMTexH1Vv_rNyja5xLUZOIazKM0DLTzbTjKlw_WYO1xvK1ICBkZ-MQ5ZnGUOjoVbKHGs1n2fwW1TccX1N39fIzfsMJWz_GI2EqOoSOF9C-Z7gOif0ReKfh_8nJBPMnEeuLtpCk6-lRUkxQui8wn6oZqFmNT8_dReiGZBzLLERfTdqz2KUnE96C8vSVD7wVXXHnxoh2wYLlRYXqdx1&csui=3):** Software (like VMware, Hyper-V, KVM) that creates and manages the virtual environments, allocating resources from the host.

**Virtual Server (Guest/VM):** Each virtual server is an independent instance, with its own operating 
system (Windows, Linux) and software, completely separate from others on
 the same host.

Key benefits

**Cost-Effective**

**Scalable & Flexible**

**Scalable & Flexible**

**Efficient Resource Use**

**Disaster Recovery**

Common uses

- Hosting websites and applications.
- Creating isolated development and testing environments.
- Running legacy applications that need older operating systems.
- Providing secure, controlled environments for sensitive tasks like email.

What is load Scalling?

adjusting system resources to maintain performance as user traffic increases (scaling up/out) or decreases (scaling down).

 It involves vertical scaling (upgrading existing server specs like 
RAM/CPU) or horizontal scaling (adding more nodes to distribute 
traffic).

Key aspects of scaling loads:

- [**Horizontal Scaling](https://www.google.com/search?client=firefox-b-e&channel=entpr&q=Horizontal+Scaling&mstk=AUtExfAQcfUgNirdohavUD8Q8F4GZ5hWA_ihsGsa5XumlcmV44BQbUBvDeBNGnP3Ujnro6r9Eeil92zHsR0s-TBruJniGzA_0L984AjzEMuZ9q_HgXkLaHeeaNT72-UhLPb4bzuWjHvg7Z5p3rumait45xrHdnu-ReJFGbHZW__be9nESJw&csui=3&ved=2ahUKEwiM-9PW06GSAxUFRmcHHXDBMgEQgK4QegQIAxAB) (Scale Out):** Adding more machines or servers to the existing infrastructure to spread the workload.
- [**Vertical Scaling](https://www.google.com/search?client=firefox-b-e&channel=entpr&q=Vertical+Scaling&mstk=AUtExfAQcfUgNirdohavUD8Q8F4GZ5hWA_ihsGsa5XumlcmV44BQbUBvDeBNGnP3Ujnro6r9Eeil92zHsR0s-TBruJniGzA_0L984AjzEMuZ9q_HgXkLaHeeaNT72-UhLPb4bzuWjHvg7Z5p3rumait45xrHdnu-ReJFGbHZW__be9nESJw&csui=3&ved=2ahUKEwiM-9PW06GSAxUFRmcHHXDBMgEQgK4QegQIAxAD) (Scale Up):** Increasing the capacity of an existing server, such as boosting CPU or RAM.
- [**Auto-scaling](https://www.google.com/search?client=firefox-b-e&channel=entpr&q=Auto-scaling&mstk=AUtExfAQcfUgNirdohavUD8Q8F4GZ5hWA_ihsGsa5XumlcmV44BQbUBvDeBNGnP3Ujnro6r9Eeil92zHsR0s-TBruJniGzA_0L984AjzEMuZ9q_HgXkLaHeeaNT72-UhLPb4bzuWjHvg7Z5p3rumait45xrHdnu-ReJFGbHZW__be9nESJw&csui=3&ved=2ahUKEwiM-9PW06GSAxUFRmcHHXDBMgEQgK4QegQIAxAF):** Automatically adjusting resources based on demand, which improves resilience and reduces costs.
- **Purpose:** Ensures application stability, prevents crashes during traffic spikes, and optimizes cost.
    
    What is a node?
    
    A node is generally any physical or virtual device that is part of a larger network or system and can send, receive, or process data.
    

Is an EC2 instance a node?

**Yes.** In most AWS contexts, an **EC2 instance is considered a node**.

- **Kubernetes (EKS):** In an Amazon EKS cluster, worker nodes are EC2 instances that run your containerized applications.
- **Big Data (EMR):** Amazon EMR clusters use EC2 instances as "Primary," "Core," or "Task" nodes to process data.
- **High-Performance Computing (PCS):** AWS Parallel Computing Service (PCS) refers to groups of EC2 instances as "compute node groups".

2. Is a subnet a node?

**No.** A subnet is **not a node**.

- A **subnet** is a range of IP addresses within a Virtual Private Cloud (VPC) that acts as a logical partition of your network.
- **Nodes (like EC2 instances) live *inside* subnets.** You launch a node into a specific subnet to define its location within an Availability Zone and its networking rules.

A **cloud provider i**s a third-party company that delivers scalable computing resources—such as 
servers, storage, databases, networking, and software applications—over 
the internet - Mtlb AWS

What is meant by jenkins?

**Jenkins plugin**

is a self-contained software add-on that extends the core functionality
 of the Jenkins automation server. Because Jenkins is a lightweight 
engine by default, it relies on these plugins to integrate with other 
tools and perform specific tasks in a CI/CD pipeline.

Key Functions

- **Integration:** Connects Jenkins to external tools like **GitHub** for source code, **Docker** for containerization, or **AWS/Azure** for cloud deployment.
- **Capability Extension:** Adds new features such as advanced build reporting, code quality
analysis (e.g., SonarQube), or instant notifications (e.g., Slack).
- **Workflow Customization:** Allows users to tailor their environment by only installing the
specific tools they need, keeping the core system stable and small.

Configure is computing to arrange computer equipment for a particular task

Configuring Jenkins Plugin for cloud provider(AWS) (for auto scalable loads) = [https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/](https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/)

You’re telling **Jenkins** how to **create and destroy cloud VMs automatically** to run jobs when load increases (auto-scaling build agents).

### 1. **Cloud**

*“Which cloud should Jenkins use to create machines?”*

- You choose a **cloud provider plugin**
- Examples:
    - AWS EC2
    - Azure
    - GCP
    - Docker
- Jenkins itself **does not create servers**
- Plugins give Jenkins that power

### 2. **Name**

Give a meaningful name for label used in Inside Jenkins plugin

1. Cloud Details - Manage Jenkins→ Credentials

must provide **cloud credentials** so Jenkins can:

- Launch instances
- Stop instances
- Terminate instances

Examples:

- AWS Access Key + Secret
- IAM Role
- Azure Service Principal
1. Region/Endpoint - which data center?
2. Real world implementation→ Good to Know

 **AMI / Image / Template**

*“What kind of machine should Jenkins create?”*

This is **VERY IMPORTANT**

You must specify:

- Base OS image (AMI / VM Image)
- Preinstalled software:
    - Java
    - Docker
    - Git
    - Build tools

Jenkins **clones this image** whenever load increases.

Action:

- Create a VM manually
- Install Java + agent dependencies
- Convert it into an image
- Use that image here
1. Select instance type and size as per need

Pick based on workload (builds vs tests)

1. Remote FS root - set a clear path
2. Add a meaningful label.
3. Exedcuters how many jobs can run on one agent at the same time ? safest is = 1

Agent = worker machine that executes build steps

- Jenkins = **Manager**
- Job = **Task**
- Agent = **Worker**
- Cloud = **Hiring agency**
1. Idle termination time of agent(This is how **auto-scaling saves money)**
2. Max no. of agents (for saving expenses)
3. Connection Method- EC2 ssh is okk
4. TEST CONFIGURATION

This auto scalling

Job queued
↓
Jenkins sees no free agent
↓
Jenkins asks cloud plugin
↓
Cloud plugin creates VM
↓
Jenkins connects via SSH
↓
Job runs
↓
Idle time reached
↓
VM destroyed

- In AWS + Jenkins, an **agent** is an **EC2 instance that Jenkins launches to run your build commands**.
- Jenkins controller schedules jobs; the **EC2 agent actually executes them** (git, build, test, deploy).
- A **VM (Virtual Machine)** is a **software-based computer** running on a physical server.
- In AWS, a VM is an **EC2 instance** — it has its own OS, CPU, RAM, disk, and IP.

[](https://www.notion.so/2f2e31ead6108094b4fcd1e210fc154e?pvs=21)