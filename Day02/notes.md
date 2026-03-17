# Day 2 – SDLC (Software Development Life Cycle)

## 1. What is SDLC?

SDLC stands for Software Development Life Cycle.

### Simple Definition

SDLC is a standard process used by software companies to design, develop, test, and deliver high-quality software.

Every company follows this process, including:

- Startups  
- MNCs  
- Product companies  

Examples:

- Amazon  
- Flipkart  
- Netflix  

All follow SDLC.

---

# 2. Goal of SDLC

The main goals are:

- Deliver high-quality software  
- Meet customer requirements  
- Reduce bugs and failures  

Example:

If software is released without testing, customers may experience:

- crashes  
- errors  
- security issues  

Therefore, SDLC ensures structured development.

---

# 3. SDLC Phases (Important)

There are six major phases in SDLC.

1. Planning  
2. Requirements  
3. Design  
4. Development / Build  
5. Testing  
6. Deployment  

It works in a cycle because new features are continuously added.

---

# 4. Example to Understand SDLC

Imagine an e-commerce company similar to Amazon.

Assume a website called:

example.com

Currently they sell:

- Men's clothes  
- Women's clothes  

Now they want to add:

Kids clothing section.

To add this feature they follow the SDLC process.

---

# 5. Phase 1 — Planning

This is the starting stage.

In this phase companies decide:

- Should we build this feature?  
- Will customers use it?  
- Is it profitable?  

### Who Works in This Phase

- Product Owner  
- Business Analyst  
- Senior Management  

### Example Questions

- Do customers want kids clothing?  
- What age group should be targeted?  
- Is there demand in the market?  

If there is no demand, the project stops here.

---

# 6. Phase 2 — Requirements Gathering

In this phase the team collects detailed requirements.

Example:

Customers want kids clothes for:

- 1–4 years  
- 6–12 years  

All information is documented in a file called:

SRS Document

SRS stands for Software Requirement Specification.

This document includes:

- features  
- functionality  
- customer needs  

---

# 7. Phase 3 — Design

After requirements are finalized, the architecture of the system is designed.

There are two types of design.

## High Level Design (HLD)

HLD describes the overall system architecture.

Examples include:

- Which database to use  
- How many servers are required  
- System scalability  
- Load balancing  
- Availability  

Example decisions:

- Use MySQL database  
- Deploy multiple servers  
- Ensure high availability  

## Low Level Design (LLD)

LLD describes the technical details of the application.

Examples include:

- functions  
- modules  
- API calls  
- database queries  

Example:

- Which Python or Java function should be called  
- What arguments should be passed  
- What response should be returned  

---

# 8. Phase 4 — Development (Build)

In this phase developers start writing code.

Steps involved:

1. Developer reads requirements  
2. Developer writes code  
3. Code is reviewed with the team  
4. Code is pushed to a repository  

Code is stored in a Source Code Repository.

Common tool used:

Git

### Purpose of Git

- Store code  
- Share code with the team  
- Track changes  

---

# 9. Phase 5 — Testing

After development the application must be tested.

A developer saying "It works on my laptop" does not mean it works everywhere.

### Who Tests the Software

QA Engineers

QA stands for Quality Assurance.

They check:

- bugs  
- errors  
- functionality  
- security  

The software is tested in different environments such as:

- Development server  
- Staging server  
- Testing environment  

---

# 10. Phase 6 — Deployment

After successful testing the software is released to production.

Production refers to the live server where customers access the application.

Example:

Customers can now buy kids clothes from the website.

---

# 11. SDLC Cycle

SDLC works as a cycle.

Planning → Requirements → Design → Development → Testing → Deployment → Repeat

Every new feature follows the same cycle.

---

# 12. Where DevOps Comes Into This

DevOps mainly focuses on three phases of SDLC.

1. Build  
2. Test  
3. Deploy  

These phases are the most important for DevOps engineers.

---

# 13. What DevOps Engineers Do

Developers write code manually.

Testers test manually.

Deployment used to be manual.

DevOps automates these steps.

| Phase | DevOps Role |
|------|-------------|
| Build | Automate builds |
| Testing | Automate testing |
| Deployment | Automate deployment |

---

# 14. Example Without DevOps

Manual process:

Developer → Push code  
Tester → Test manually  
Admin → Deploy manually  

Problems:

- slow process  
- human errors  
- miscommunication  

---

# 15. Example With DevOps

Automated pipeline:

Developer → Push code → Pipeline runs automatically

Steps happen automatically:

1. Build  
2. Test  
3. Deploy  

Tools used include:

- Jenkins  
- GitHub Actions  
- GitLab CI/CD  

This process is called:

CI/CD

Continuous Integration  
Continuous Delivery

---

# 16. DevOps Main Goal

DevOps engineers aim to:

- Automate building  
- Automate testing  
- Automate deployment  

Result:

- Faster software delivery  
- Less manual work  
- Higher efficiency  

---

# 17. SDLC Models

There are different ways to implement SDLC.

Common models include:

1. Waterfall Model  
2. Iterative Model  
3. Agile Model  

Most companies today use:

Agile Methodology

In Agile:

Work is divided into small sprints and features are released quickly.

---

# 18. Interview Question (Important)

If an interviewer asks:

Which SDLC phases are important for DevOps engineers?

Answer:

DevOps engineers mainly focus on automating the build, testing, and deployment phases of the software development lifecycle to improve delivery speed and efficiency.

---

# 19. Simple Summary

SDLC is the process used to build and deliver software.

Steps involved:

1. Planning  
2. Requirements  
3. Design  
4. Development  
5. Testing  
6. Deployment  

DevOps focuses on automating the build, testing, and deployment phases.