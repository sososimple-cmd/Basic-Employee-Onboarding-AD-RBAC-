# Basic Employee Onboarding | Active Directory & RBAC
Active Directory infrastructure rebuild for Northstar Medical Group, a fictional healthcare organization. This project includes domain setup, organizational structure, user provisioning, RBAC implementation, and incident resolution.
## Problem Statement

Northstar Medical Group inherited an Active Directory environment that had been poorly managed by its previous managed service provider (MSP). Employee identities were handled through manual processes with no consistent naming standards, organized OU structure, or reliable method for assigning access. This made onboarding difficult to manage and increased the possibility of users receiving missing or inappropriate permissions. For a healthcare organization with more than 200 employees, these identity-management gaps also created security and potential HIPAA compliance risks.

## Solution Overview

I built the NMG.com domain from scratch using Windows Server 2019 and promoted NMG-DC01 to a domain controller. I created department-based OUs for Finance, HR, IT, and Operations to keep identities organized and support consistent policy application.

I also created a global security group for each department and implemented a flat RBAC model to assign access based on business roles. I provisioned 15 fictional employee identities using consistent usernames, UPNs, job titles, and department attributes. Each user was placed in the correct OU and assigned to the appropriate security group.

Finally, I tested the environment by investigating and resolving ticket NMG-0047, which involved multiple configuration problems affecting an HR Payroll Specialist.
## Video Walkthrough

🎥 [Watch My Active Directory Project Walkthrough](https://youtu.be/pg_NZQtr96s) 

The walkthrough demonstrates the NMG.com domain, department OUs, security groups, user provisioning, RBAC assignments, and my investigation and resolution of ticket NMG-0047.

## Tools Used

* Windows Server 2019

* Active Directory Domain Services

* VirtualBox

* Role-Based Access Control (RBAC)

* Jira-style ticket documentation

* GitHub

## Project Timeline

Day 1: Domain creation and domain controller promotion

Day 2: Organizational unit and security group design

Day 3: User provisioning and RBAC implementation

Day 4: Incident response and resolution (NMG-0047)

Day 5: Documentation and case study packaging

## Key Accomplishments

* Built the NMG.com Active Directory domain from scratch and validated the domain controller

* Designed four department-based OUs and four Global Security groups to support a scalable flat RBAC model

* Provisioned 15 employee identities using consistent usernames, UPNs, job titles, and department attributes

* Assigned department access through security groups instead of individual user permissions

* Diagnosed four connected identity issues affecting jcooper: incorrect OU, group membership, job title, and department

* Corrected Julissa Cooper's identity to match her HR Payroll Specialist role and removed inappropriate Operations access

* Documented the investigation, root cause, remediation, and verification in an audit-friendly resolution report
