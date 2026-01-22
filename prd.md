# Product Requirements Document: CareNexa MVP

**Author:** Thomas Perdana
**Date:** Jan 22, 2026

## 1. Introduction

This document outlines the product requirements for the Minimum Viable Product (MVP) of **CareNexa**, a comprehensive, multi-division healthcare SaaS platform. The project was initiated by a solo founder with a background as a Registered Nurse (RN) and healthcare operator. The objective is to create a unified healthcare operating system that streamlines operations for agencies across a wide range of service areas, from homecare and behavioral health to MedSpa and transportation services. The founder will provide a complete blueprint, including all necessary workflows, service requirements, and documentation templates, to guide the development process.

## 2. Goals and Objectives

The primary goal is to develop a functional and scalable MVP of the CareNexa platform within a **4-month timeframe**. This MVP will serve as the foundation for a full-featured healthcare operating system.

### Key Business Objectives:

*   **Centralize Operations:** Bring scheduling, documentation, billing, staff management, and compliance into a single, integrated platform.
*   **Support Diverse Services:** Cater to the unique operational needs of multiple healthcare divisions.
*   **Improve Efficiency:** Automate and streamline workflows for agency owners, staff, and administrators.
*   **Ensure Scalability:** Build a robust, multi-tenant architecture capable of supporting numerous agencies.

### Key Technical Objectives:

*   Deliver a clean, modular, and well-documented codebase.
*   Implement a secure, multi-tenant architecture to ensure data isolation between agencies.
*   Develop a role-based access control system to manage user permissions effectively.
*   Ensure the platform is developed with HIPAA compliance considerations in mind.

## 3. User Personas and Target Audience

The platform will serve various roles within a healthcare agency. The MVP will focus on providing distinct experiences and permissions for the following user personas:

| User Persona      | Description                                                                                             | Key Needs                                                                                                  |
| ----------------- | ------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Admin**         | The superuser with full access to the platform, responsible for system-wide configuration and management. | Complete control over all platform settings, agency management, and user roles.                            |
| **Agency Owner**  | Manages a specific agency on the platform, overseeing staff, clients, billing, and overall operations.    | Onboarding staff/clients, managing schedules, viewing dashboards, and generating billing reports.             |
| **Staff**         | Frontline service providers who use the system for scheduling, documentation, and communication.         | Accessing schedules, completing service documentation, internal messaging, and receiving alerts.            |

*Note: The "Staff" persona encompasses a wide variety of roles, including DSP, HHA, RN, LPN, BCBA, Driver, and MedSpa Clinician. The system must accommodate the specific needs of each role through tailored permissions and workflows.*

## 4. Features and Functionality (MVP Scope)

The MVP will be built over four months and will include the following core feature sets:

### 4.1. Authentication & Multi-Role Access
*   Secure user login and authentication.
*   Multi-tenant architecture to isolate each agency's data and environment.
*   Role-Based Access Control (RBAC) for the defined user personas (Admin, Agency Owner, Staff).

### 4.2. Agency & Staff Management
*   Onboarding workflows for new agencies, staff members, and clients.
*   Functionality to assign specific services to clients.
*   A centralized document management system for uploading and storing essential files (e.g., certifications, contracts).

### 4.3. Scheduling System
*   A comprehensive scheduling module that supports:
    *   Staff shift scheduling.
    *   Client appointment scheduling.
    *   Attendance tracking for Day Habilitation programs.
    *   Visit scheduling for Homecare services.
    *   Route management for Transportation services.
    *   Appointment booking for MedSpa clinics.

### 4.4. Documentation Workflows
*   A dynamic documentation system with customizable templates for each service type. This includes, but is not limited to:
    *   AT evaluations & training notes
    *   Respite, CBS, and Individual Supports notes
    *   Dayhab and Residential logs
    *   Homecare nursing and Behavioral notes
    *   MedSpa treatment notes

### 4.5. Billing Module (Basic)
*   Tracking of service units and creation of service logs.
*   Generation of exportable billing reports (e.g., CSV, PDF).
*   Basic claims preparation functionality. **Note:** Direct clearinghouse integration is out of scope for the MVP.

### 4.6. Dashboards
*   Role-specific dashboards to provide at-a-glance insights:
    *   **Agency Dashboard:** Overview of key operational metrics.
    *   **Staff Dashboard:** View of personal schedules, tasks, and pending documentation.
    *   **RN Dashboard:** Specialized view for nursing-specific tasks and oversight.
    *   **MedSpa Dashboard:** Metrics and schedules relevant to aesthetic clinic operations.

### 4.7. Messaging & Notifications
*   An internal messaging system for communication between platform users.
*   Automated alerts and notifications for schedule changes, upcoming tasks, and documentation deadlines.

## 5. Technical Requirements

| Category          | Requirement                                                                                                                                                                                                                                                                                       |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**      | **React** (with TypeScript and TanStack) is recommended for a modern, component-based UI.                                                                                                                                                                                                          |
| **Backend**       | **Node.js** (with TypeScript) is recommended for its performance and alignment with a JavaScript-based frontend.                                                                                                                                                                                  |
| **Database**      | **PostgreSQL** is recommended for its robustness, scalability, and strong support for complex queries.                                                                                                                                                                                            |
| **UI/UX**         | The UI should be clean, modern, and intuitive, following an Apple macOS style with switchable dark blue gradient and muted brownish light themes. Shadcn UI components should be used for consistency and quality. Animations and infographics should be used to enhance the user experience. |
| **Hosting**       | The application should be deployed on a scalable cloud provider like **Vercel** or **AWS**.                                                                                                                                                                                                      |
| **Version Control** | All code will be managed in a **GitHub** repository owned by the client.                                                                                                                                                                                                                          |
| **Architecture**  | The system must be built on a **clean, modular, and scalable architecture**. A multi-tenant database schema is required.                                                                                                                                                                             |
| **Compliance**    | Development must be **HIPAA-aware**, implementing necessary safeguards to protect patient health information (PHI).                                                                                                                                                                                 |

## 6. Assumptions and Constraints

*   **Assumption:** The client will provide a complete and detailed project blueprint, including all workflows, forms, and service requirements, prior to the start of each milestone.
*   **Constraint:** The MVP must be completed within a strict **4-month (16-week) timeline**.
*   **Constraint:** The project budget is fixed between **$15,000 and $25,000**.
*   **Constraint:** The development process will follow a **milestone-based delivery** schedule with mandatory weekly demos.
*   **Constraint:** All communication and project management will be conducted through Upwork messages and weekly video calls.

## 7. Success Metrics

The success of the CareNexa MVP will be measured by the following criteria:

*   **On-Time Delivery:** Successful completion and deployment of the MVP within the 16-week timeframe.
*   **Scope Completion:** All features outlined in Section 4 are implemented, functional, and meet the specified requirements.
*   **Code Quality:** The codebase is clean, well-documented, scalable, and adheres to the architectural principles outlined.
*   **Client Satisfaction:** Positive feedback and acceptance of deliverables during weekly demos and at the final project handover.
*   **System Stability:** The platform is stable and performs reliably in a production environment.

## 8. Timeline and Milestones

A high-level timeline is proposed below. This will be finalized in collaboration with the client.

| Milestone | Month | Key Deliverables                                                                                                                                                           |
| :-------- | :---- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1**     | 1     | - **Foundation & Auth:** Setup project, database, and hosting. Implement multi-tenant auth and role-based access.<br>- **Onboarding:** Build agency, staff, and client onboarding workflows. |
| **2**     | 2     | - **Core Scheduling:** Develop the comprehensive scheduling system for all service types.<br>- **Documentation V1:** Implement the dynamic documentation template engine.             |
| **3**     | 3     | - **Documentation V2:** Complete all required documentation workflows.<br>- **Billing Module:** Build the basic billing module with unit tracking and reporting.                  |
| **4**     | 4     | - **Dashboards & Messaging:** Create all role-based dashboards and the internal messaging system.<br>- **Testing & Deployment:** Conduct thorough end-to-end testing, bug fixing, and deploy the MVP. |
