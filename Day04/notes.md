# Day 4 – Servers, Virtual Machines, and Virtualization

## 1. What Will Be Covered in This Session

- What is a Server
- What are Physical Servers
- What is a Virtual Machine (VM)
- What is a Hypervisor
- How virtual machines work in real-world scenarios
- How cloud providers like AWS create virtual machines

The goal is to understand virtualization using a simple real-world example.

---

# 2. Real-World Example (Land Example)

Imagine you have:

1 acre of land.

You build a large house and live there with your family.

### Situation

You realize that your family only needs half an acre.

The other half acre remains unused.

This means resources are being wasted.

### Better Solution

You decide to:

- Build another house on the unused land
- Rent it to another family

Now:

- You still live comfortably
- Another family lives there
- The land is used efficiently
- You earn rent

### Key Concept

| Situation | Result |
|----------|--------|
| Whole land used by one family | Inefficient |
| Land divided and rented | Efficient |

This represents the concept of resource optimization.

---

# 3. DevOps Principle

A core principle of DevOps is improving efficiency.

DevOps aims to:

- Use resources efficiently
- Reduce wastage
- Automate systems
- Improve infrastructure utilization

---

# 4. Converting the Example to IT Infrastructure

Instead of land, consider servers.

## What is a Server?

A server is a computer where applications are deployed so users can access them through the internet.

Examples:

- google.com
- amazon.com

These websites run on servers inside data centers.

---

# 5. Example of Physical Servers

Suppose a company called:

example.com

buys 5 physical servers from hardware companies such as:

- HP
- IBM

Servers:

- Server 1
- Server 2
- Server 3
- Server 4
- Server 5

Each server may have very large capacity.

Example specifications:

- 100 GB RAM
- 100 CPU cores

---

# 6. The Resource Waste Problem

A team deploys an application.

Application: App 1

Requirements:

- 4 GB RAM
- 4 CPU cores

But the server has:

- 100 GB RAM
- 100 CPU cores

### Resource Usage

| Resource | Used | Unused |
|---------|------|--------|
| RAM | 4 GB | 96 GB |
| CPU | 4 cores | 96 cores |

This means most of the server resources remain unused.

---

# 7. Multiple Teams Scenario

Imagine 5 teams in a company.

Each team receives one physical server.

But their applications may use only about 10% of the server resources.

Therefore:

- 90% of the resources remain unused.

This creates infrastructure inefficiency.

---

# 8. Solution: Virtualization

To solve this problem, virtualization was introduced.

Instead of assigning one physical server to one team:

The server is logically divided.

This creates multiple virtual machines.

---

# 9. What is a Virtual Machine?

A Virtual Machine (VM) is a logical computer created inside a physical server.

Example:

One physical server can create:

- VM1
- VM2
- VM3
- VM4
- VM5

Each VM behaves like an independent computer.

### Important Point

The server is not physically divided.

It is logically divided.

This concept is known as logical isolation.

---

# 10. What is a Hypervisor?

A hypervisor is software that creates and manages virtual machines.

Definition:

A hypervisor is software that runs on a physical server and creates multiple virtual machines.

---

# 11. Popular Hypervisors

Some well-known hypervisors include:

- VMware
- Xen

These technologies allow multiple virtual machines to run on a single physical server.

---

# 12. How Virtual Machines Work

Example setup:

Physical Server → Hypervisor installed

The hypervisor creates:

- Virtual Machine 1
- Virtual Machine 2
- Virtual Machine 3
- Virtual Machine 4
- Virtual Machine 5

Each virtual machine has its own:

- CPU
- RAM
- Storage
- Operating System

However, all of them run on the same physical machine.

---

# 13. Cloud Providers and Virtual Machines

Cloud providers such as:

- Amazon Web Services (AWS)
- Microsoft Azure
- Google Cloud

use virtualization technology.

They build large data centers.

Inside these data centers:

- thousands of physical servers
- hypervisors installed on those servers

These servers create virtual machines for customers.

---

# 14. Example: AWS Data Centers

AWS operates data centers in multiple regions.

Examples include:

- Mumbai
- Singapore
- Ohio (USA)

Companies select regions depending on user location to reduce latency.

---

# 15. What is Latency?

Latency refers to the delay in communication between a user and a server.

Example:

If a user in India accesses a server in:

Mumbai → Low latency

Ohio → Higher latency

Therefore cloud providers place data centers around the world.

---

# 16. Inside an AWS Data Center

Inside a data center there are:

- Racks
- Physical servers

Example:

Physical Server 1  
Physical Server 2  
Physical Server 3  
Physical Server 100

Each server may have very large resources.

Example:

- 100 GB RAM
- 100 CPU cores

---

# 17. Creating a Virtual Machine on AWS

Suppose a DevOps engineer requests a virtual machine.

Requested configuration:

- 10 GB RAM
- 12 CPU cores

### Steps

1. User logs into AWS.
2. User requests a VM in the Mumbai region.
3. AWS receives the request.
4. AWS finds a suitable physical server.
5. The hypervisor creates the VM.
6. AWS sends access details to the user.

---

# 18. Information Provided to the User

The user receives:

- IP address
- Login credentials
- Key pair

Using these details, the user can connect to the virtual machine remotely.

---

# 19. Important Limitation

Even though a user pays AWS for the virtual machine:

The user does not own the physical server.

The user only gets logical access to the virtual machine.

The physical server remains inside AWS data centers.

---

# 20. Efficiency Improvement

Without virtualization:

100 physical servers → 100 users

With virtualization:

100 physical servers → millions of virtual machines

This greatly improves resource efficiency.

---

# 21. Virtualization on Personal Computers

Virtual machines can also run on personal computers.

Example tool:

Oracle VirtualBox

Using this tool:

A single laptop can run multiple operating systems.

Different users can use separate virtual environments.

---

# 22. Final Concept Summary

Virtual machines are:

- Virtual computer systems
- Created from physical servers
- Managed by hypervisors
- Used by cloud providers
- Designed to improve resource efficiency