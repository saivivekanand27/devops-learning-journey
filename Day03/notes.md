# Day 3 – DevOps Roles and Task Flow in an Organization

## 1. Main Question of This Topic

The instructor answers an important question:

If you join a company as a DevOps engineer, where do your tasks come from?

Important point:

- DevOps engineers do not talk directly to customers.
- DevOps engineers do not decide product features.

Instead, requirements flow through multiple roles before reaching DevOps engineers.

---

# 2. Example Organization

Example company: Amazon

Inside Amazon there are multiple projects such as:

- Amazon Fresh
- Amazon Prime
- Amazon E-commerce
- Amazon Home Services

Even if an offer letter says Amazon, an employee typically works on one project.

Example:

A DevOps engineer may work on Amazon Fresh.

---

# 3. Roles Inside an Organization

Many roles are involved in building software.

Requirement flow:

Customer → Business Analyst → Product Manager → Product Owner → Solution Architect → Development Team → DevOps / QA / DBA

Each role contributes to building the product.

---

# 4. Customer (Start of Requirement)

Everything starts from customers.

Example request:

A customer suggests that it would be useful if Amazon Fresh delivers groceries in 15 minutes.

This becomes a new product idea.

Customers do not communicate directly with engineers.

---

# 5. Business Analyst (BA)

The Business Analyst collects requirements from customers.

Responsibilities:

- Talk to customers
- Understand problems
- Convert ideas into documents

They create a document called:

BRD – Business Requirement Document

Example BRD:

Feature: 15-minute grocery delivery

Another example:

Customer request: Add UPI payment option.

The Business Analyst writes a BRD for this feature.

---

# 6. Product Manager (PM)

The Product Manager decides which features are most important.

Example:

Two feature requests:

1. 15-minute delivery  
2. New payment gateway

The Product Manager may decide to implement the 15-minute delivery feature first in Q1 (January to March).

Product Managers prioritize work.

---

# 7. Product Owner (PO)

The Product Owner takes the feature and breaks it into smaller tasks.

Example feature:

15-minute delivery

The Product Owner divides it into tasks such as:

- Mobile application UI
- Backend API
- Delivery algorithm
- Database changes

These tasks are called Epics.

Epics are further broken into smaller tasks called Stories.

---

# 8. Solution Architect

The Solution Architect designs the technical solution.

They create system designs including:

High Level Design (HLD)

High Level Design describes the overall architecture of the system.

Examples:

- Which architecture to use
- Which database to use
- How scaling will work

Low Level Design (LLD)

Low Level Design describes technical implementation details.

Examples:

- APIs
- Modules
- Frameworks
- Microservices

After design is finalized, the development team begins work.

---

# 9. Development Team

The development team includes:

- Developers
- DevOps engineers
- QA engineers
- Database administrators
- Technical writers

Together they form a Scrum Team.

The Scrum Team works together to complete the feature.

---

# 10. Role of Developers

Developers analyze requirements and write application code.

Example infrastructure needs:

- Kubernetes cluster
- Docker containers
- Git repository
- Cloud infrastructure
- Database

Developers request infrastructure from DevOps engineers.

This is where DevOps engineers begin receiving tasks.

---

# 11. DevOps Engineer Tasks

DevOps engineers provide infrastructure and automation.

Typical tasks include:

- Creating Kubernetes clusters
- Setting up Docker environments
- Creating CI/CD pipelines
- Setting up Git repositories
- Provisioning AWS infrastructure
- Configuring servers

DevOps engineers support developers by enabling efficient software delivery.

---

# 12. QA Engineers

QA engineers test the application.

They verify:

- Bugs
- Errors
- Functionality
- Performance

Their goal is to ensure the quality of the software.

---

# 13. Database Administrator (DBA)

Database Administrators manage databases.

Responsibilities include:

- Creating databases
- Optimizing queries
- Performing backups
- Improving database performance

---

# 14. Technical Writers

Technical writers create documentation for software features.

Example:

When Android releases a new feature, documentation explains:

- What the feature does
- How users can use it

Companies document features in a similar way.

---

# 15. Site Reliability Engineers (SRE)

After the product goes live, SRE engineers ensure:

- System reliability
- High uptime
- Monitoring
- Alerting

They create dashboards and alerts to monitor system health.

---

# 16. Summary of Roles

Requirement flow:

Customer  
↓  
Business Analyst  
↓  
Product Manager  
↓  
Product Owner  
↓  
Solution Architect  
↓  
Scrum Team (Developers + DevOps + QA + DBA)

---

# 17. Software Development Life Cycle (SDLC)

All these roles work within the Software Development Life Cycle.

Typical SDLC stages:

1. Planning  
2. Analysis  
3. Design  
4. Implementation  
5. Testing  
6. Deployment  
7. Maintenance

---

# 18. What DevOps Engineers Improve

DevOps engineers focus on improving development efficiency.

Example:

If development takes three months, DevOps engineers aim to reduce it to two months.

They achieve this through automation.

Examples:

- CI/CD pipelines
- Automated testing
- Automated deployments
- Security scanning

---

# 19. What is Jira?

Jira is a project management tool used by many companies.

Created by Atlassian.

Purpose:

- Track tasks
- Assign work
- Monitor progress
- Manage projects

Many software teams rely on Jira.

---

# 20. Why Jira is Needed

Example scenario:

A DevOps engineer is creating a Kubernetes cluster.

If the task is blocked:

- Developers cannot continue development
- QA cannot test
- Project deadlines may be affected

Jira helps management track:

- Who is working on which task
- Which tasks are blocked
- Overall project progress

---

# 21. Important Jira Concepts

Epic

A large feature.

Example: 15-minute delivery system.

Story

A smaller task inside an epic.

Examples:

- Mobile UI
- Backend API
- Kubernetes cluster setup

Sprint

A sprint is a short development cycle of 2–3 weeks.

Example Sprint Tasks:

- Create Kubernetes cluster
- Setup CI/CD
- Build API

At the end of the sprint, the team reviews progress.

---

# 22. Sprint Process

Typical sprint workflow:

1. Sprint planning  
2. Work on assigned tasks  
3. Daily updates  
4. Sprint review  
5. Sprint retrospective

This process follows Agile methodology.

---

# 23. How DevOps Engineers Receive Tasks in Jira

Example Jira stories:

Task: Create Kubernetes cluster using Terraform  
Assigned to: DevOps engineer

Task: Setup AWS RDS database  
Assigned to: DevOps engineer

DevOps engineers update progress regularly.

Example updates:

Day 1 – Terraform code written  
Day 2 – Cluster provisioning in progress  
Day 3 – Cluster successfully deployed

This allows the entire team to track progress.

---

# 24. Daily DevOps Work

Typical daily tasks of a DevOps engineer:

- Check Jira tasks
- Work on infrastructure
- Write automation scripts
- Update CI/CD pipelines
- Monitor systems
- Update task progress in Jira

---

# 25. Key Idea

DevOps engineers do not receive tasks directly from customers.

Tasks flow through multiple roles:

Customer → Business Analyst → Product Manager → Product Owner → Solution Architect → Developers → DevOps

All tasks are tracked in Jira.

---

# 26. Simple Summary

DevOps engineers:

- Automate infrastructure
- Support developers
- Improve SDLC efficiency
- Track work through Jira