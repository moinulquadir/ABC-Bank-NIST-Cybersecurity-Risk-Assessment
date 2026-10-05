# ISMS Scope and Boundary Matrix

**Organization:** Northstar Software Labs (fictional)  
**ISMS Version:** 1.0  
**Status:** Approved for portfolio simulation

## Scope Statement
The ISMS covers the people, processes, information, applications, cloud infrastructure, endpoints, offices, suppliers, and security operations used to design, develop, operate, support, and administer Northstar's AWS-hosted B2B workflow SaaS platform and the corporate services that support it.

## In Scope
| Area | Included | Boundary / Notes |
|---|---|---|
| SaaS production | Yes | Application, APIs, databases, storage, production monitoring |
| AWS environment | Yes | Accounts, IAM, networking, compute, managed services used by SaaS |
| Corporate IT | Yes | Identity, endpoint management, collaboration, ticketing |
| Employees/contractors | Yes | Personnel with access to in-scope information or systems |
| Secure SDLC | Yes | Planning, coding, review, testing, release |
| Customer support | Yes | Support workflows and access to customer information |
| Security operations | Yes | Logging, monitoring, vulnerability and incident management |
| Key suppliers | Yes | Suppliers that host, process, transmit, or materially support in-scope services |
| New York office | Yes | Corporate workspace and network/security processes |
| Remote work | Yes | Company-approved remote access and endpoints |

## Out of Scope / Boundary
| Area | Status | Rationale / Treatment |
|---|---|---|
| Customer-owned endpoints | Outside | Customer responsibility; Northstar addresses its service interface and contractual obligations |
| Customer internal networks | Outside | Not administered by Northstar |
| Personal devices without company data/access | Outside | Must not be used for in-scope processing unless approved |
| Supplier internal operations | Outside boundary | Supplier security is addressed through due diligence and contractual controls |
| Future products not yet launched | Outside current scope | Added through formal scope review when introduced |

## Interfaces and Dependencies
AWS, identity provider, code repository, CI/CD platform, ticketing platform, endpoint-management service, email/collaboration service, payment/customer support suppliers, and critical SaaS vendors are treated as dependencies and evaluated through risk and supplier-management processes.

## Scope Review Triggers
Material acquisitions, new products, major architecture changes, significant supplier changes, regulatory/contractual changes, or major risk changes trigger a scope review.
