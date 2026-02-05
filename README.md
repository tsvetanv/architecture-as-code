# Architecture as Code (AaC): Automate Your Software Architecture

This repository is the **entry point and public hub** for my presentation  
**“Architecture as Code (AaC): Automate Your Software Architecture”**.

It provides a short explanation of the concept, and links to the full demo system repositories, architecture artifacts, and resources.

---

## 1. Introduction: What is Architecture as Code (AaC)?

**Architecture as Code (AaC)** is the practice of treating software architecture as a **version-controlled, continuously evolving, and automatable artifact**, rather than a static set of diagrams created once at the beginning.

Instead of:
> draw → implement → forget

AaC promotes:
> define → version → validate → evolve

Architecture becomes **executable knowledge** that can be:
- stored in Git
- reviewed through pull requests
- validated automatically
- kept aligned with implementation and infrastructure

The main goal is to reduce **architecture drift** and make architecture a living part of software delivery.

---

## 2. Purpose of This Repository

This repository exists as a **central hub** for my public presentation and its related demo project.

- Event page (DEV.BG):  
https://dev.bg/event/architecture-as-code-aac-automate-your-software-architecture/
- Presentation slides (PowerPoint):  
[20260120-Architecture-as-Code-TsvetanVasilev-DevBG.pptx](./20260120-Architecture-as-Code-TsvetanVasilev-DevBG.pptx)

---

## 3. Presentation Agenda

The talk is structured around the following topics:

- Why traditional architecture breaks
- What Architecture-as-Code really means
- How it works in practice
- Trade-offs, costs, and when it makes sense

---

## 4. Demo Project: Order Processing System (OPS)

To demonstrate Architecture as Code in practice, the presentation is supported by a demo system called:

### **Order Processing System (OPS)**

OPS is a production-inspired backend system that demonstrates:
- modular structure and clear boundaries
- explicit architectural decisions (ADRs)
- C4 model diagrams generated from code (Structurizr DSL)
- infrastructure described as code (Terraform)
- architecture documentation as a first-class deliverable

### Main Functionalities

The demo system supports the following core business use cases:

- Create Order
- Process Order
- Track Order Status
- Cancel Order

---

## 5. OPS Repositories and Project Board

The demo is implemented as multiple repositories, each with a clear responsibility.

### 1) Architecture Repository (Source of Truth)
https://github.com/tsvetanv/order-system-architecture

Contains:
- Structurizr DSL workspace (C4 model diagrams)
- arc42-based documentation structure
- architecture decisions and architecture artifacts

---

### 2) Services Repository (Application Implementation)
https://github.com/tsvetanv/order-system-services

Contains:
- the actual backend implementation (Spring Boot)
- modular monolith structure
- business logic and integration layer

---

### 3) Infrastructure Repository (Terraform)
https://github.com/tsvetanv/order-system-infrastructure

Contains:
- AWS infrastructure defined with Terraform
- ECS/Fargate deployment setup
- RDS PostgreSQL infrastructure
- security and networking resources

---

### 4) GitHub Project Board (Iterative Development)
https://github.com/users/tsvetanv/projects/4

The GitHub Project represents the **iterative way of development** of the demo system and its architecture.

It tracks work items and shows how the solution evolves step-by-step, including architecture decisions and implementation progress.

---

## 6. Key Idea: Architecture evolves every sprint

Architecture is not a one-time design activity.

Even if teams do not manage architecture explicitly, it still evolves under delivery pressure.

AaC exists to make this evolution:
- visible
- versioned
- reviewable
- enforceable

---

## 7. Resources

1. Simon Brown (C4 Model): https://c4model.com/
2. Simon Brown blog: https://simonbrown.je/
3. Conference Paper: *Architecture as Code* (ICSA 2025):  https://www.researchgate.net/publication/394538438_Architecture_as_Code

---

## 8. Contacts

- LinkedIn: https://www.linkedin.com/in/tsvetanv/
- GitHub: https://github.com/tsvetanv
