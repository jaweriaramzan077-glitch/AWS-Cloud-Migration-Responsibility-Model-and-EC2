# AWS-Cloud-Migration-Responsibility-Model-and-EC2
# AWS Cloud Migration, Shared Responsibility Model & EC2

## 1. Cloud Migration – 6 R's

Cloud migration means moving applications, data, and workloads from an existing environment to the cloud.

### 1. Rehost

Rehost means moving an application to the cloud **without making major changes**.

**Example:** Moving an existing server from a local data center to AWS.

### 2. Replatform

Replatform means moving an application to the cloud with **small improvements**, but without completely changing it.

**Example:** Moving a database to a managed AWS database service.

### 3. Repurchase

Repurchase means replacing an existing application with a **new cloud-based product or service**.

**Example:** Replacing an old software system with a SaaS solution.

### 4. Refactor

Refactor means **redesigning or changing the application** to take better advantage of cloud features.

**Example:** Changing an application into cloud-native services.

### 5. Retire

Retire means **removing applications that are no longer needed** instead of moving them to the cloud.

### 6. Retain

Retain means keeping an application in its **existing environment** when migration is not currently suitable.

---

# 2. AWS Shared Responsibility Model

The AWS Shared Responsibility Model explains which security responsibilities belong to AWS and which belong to the customer.

### 1. Security OF the Cloud

AWS is responsible for **security of the cloud infrastructure**.

AWS manages:

* Physical data centers
* Hardware
* Networking infrastructure
* AWS global infrastructure

### 2. Security IN the Cloud

The customer is responsible for **security of what they run in AWS**.

Customers manage things such as:

* Data
* User access
* IAM permissions
* Operating system security
* Application security
* Security configurations

**Easy way to remember:**

**AWS → Security OF the Cloud**
**Customer → Security IN the Cloud**

---

# 3. Amazon EC2

**EC2 (Elastic Compute Cloud)** is an AWS service that provides **virtual servers in the cloud**.

An EC2 server is called an **EC2 Instance**.

You can use an EC2 instance to:

* Run applications
* Host websites
* Run software
* Store and process data
* Perform computing tasks

---

# 4. What is a Virtual Machine?

A **Virtual Machine (VM)** is a software-based computer that runs inside a physical computer.

It has its own:

* CPU resources
* Memory (RAM)
* Storage
* Operating system

An EC2 instance works like a virtual server that you can use without owning the physical server yourself.

---

# 5. Why Do We Need an EC2 Instance?

We use an EC2 instance when we need a **server for running applications or services**.

For example:

A company wants to host a website. Instead of buying a physical server, it can create an **EC2 instance on AWS** and run the website there.

### Benefits:

* Easy to create
* Flexible
* Scalable
* Pay-as-you-go
* No need to maintain physical hardware

---

# 6. Hypervisor and Virtual Instances

A **Hypervisor** is software that allows multiple virtual machines to run on a physical server.

It divides the physical server's resources, such as CPU and RAM, among different virtual machines.

**Simple example:**

Physical Server
↓
Hypervisor
↓
VM 1 | VM 2 | VM 3

In AWS, EC2 instances run on AWS's underlying physical infrastructure using virtualization technology.

---

# 7. AMI – Amazon Machine Image

**AMI (Amazon Machine Image)** is a template used to create an EC2 instance.

An AMI can contain:

* Operating system
* Applications
* Configuration
* Required software

**Easy example:**

AMI = **Ready-made template**
EC2 Instance = **Virtual server created from that template**

---

# 8. EC2 Instance Types / Families

AWS provides different EC2 instance families for different workloads.

### 1. General Purpose

Balanced combination of **CPU, memory, and networking**.

**Used for:**

* Websites
* Applications
* Development and testing

### 2. Compute Optimized

Designed for workloads that need **high CPU performance**.

**Used for:**

* Gaming servers
* High-performance applications
* Batch processing

### 3. Memory Optimized

Designed for applications that need **large amounts of RAM**.

**Used for:**

* Large databases
* Data processing
* In-memory applications

### 4. Storage Optimized

Designed for workloads that need **fast and high-volume storage access**.

**Used for:**

* Databases
* Data warehouses
* Large data processing

### 5. Accelerated Computing

Uses specialized hardware such as **GPUs or other accelerators**.

**Used for:**

* Machine learning
* AI workloads
* Graphics processing
* Scientific computing

---

# 9. EC2 Instance Size

Within an instance family, AWS provides different sizes according to the required resources.

### Small

Suitable for workloads that need fewer resources.

### Medium

Provides more CPU and memory than a small instance.

### Large

Provides more resources and is suitable for heavier workloads.

**Simple idea:**

Small → Less Resources
Medium → More Resources
Large → More Powerful

---

# Quick Revision

| Topic                 | Easy Meaning                           |
| --------------------- | -------------------------------------- |
| Rehost                | Move without major changes             |
| Replatform            | Move with small improvements           |
| Repurchase            | Replace with a new product             |
| Refactor              | Redesign for the cloud                 |
| Retire                | Remove unnecessary application         |
| Retain                | Keep it where it is                    |
| EC2                   | Cloud-based virtual server             |
| VM                    | Virtual computer                       |
| Hypervisor            | Runs multiple VMs on a physical server |
| AMI                   | Template for creating EC2 instances    |
| General Purpose       | Balanced resources                     |
| Compute Optimized     | High CPU                               |
| Memory Optimized      | High RAM                               |
| Storage Optimized     | Fast/high storage                      |
| Accelerated Computing | GPU/special hardware                   |

## Conclusion

AWS provides different migration strategies, security responsibilities, and computing options according to business requirements. EC2 makes it easy to create and manage virtual servers in the cloud, while AMIs and different instance families help users choose the right environment for their workloads.
