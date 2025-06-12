### ✅ Functional Requirements (FR)

Functional requirements describe what the system should do — its features and capabilities.

| # Cod | Requirement                                                                                          |
| ----- | ---------------------------------------------------------------------------------------------------- |
| FR01  | System must allow registration of **contractors** with profile details                               |
| FR02  | System must allow registration of **escorts** with profile details, availability, and tier selection |
| FR03  | Contractors must be able to **search** for escorts based on tier, location, and availability         |
| FR04  | Contractors must be able to **book** an escort for a specific time slot                              |
| FR05  | Escorts must be able to **accept or reject** booking requests                                        |
| FR06  | System must allow **tier-based service description** and pricing                                     |
| FR07  | System must support **secure messaging/chat** between escorts and contractors                        |
| FR08  | Escorts and contractors must have **dashboard access** to view their bookings and schedules          |
| FR09  | System must send **email/SMS notifications** for booking confirmations, changes, or cancellations    |
| FR10  | System must allow **ratings and reviews** after a completed session                                  |

Optional Advanced Functionalities (you can include later or make "future scope"):

* **FR11**: Payment system (if applicable) – integrate with Stripe/PayPal
* **FR12**: Admin panel to manage users, disputes, reports, and content moderation
* **FR13**: Geo-location services to match contractors and escorts nearby
* **FR14**: Calendar integration for booking and availability

---

### 🧱 Non-Functional Requirements (NFR)

Non-functional requirements describe **how** the system should behave — qualities like performance, security, and maintainability.

| # Cod | Requirement                                                                          |
| ----- | ------------------------------------------------------------------------------------ |
| NFR01 | Must be a web-based application, mobile responsive                                   |
| NFR02 | System must handle at least 1,000 concurrent users (scalability)                     |
| NFR03 | System must ensure secure user authentication and authorization                      |
| NFR04 | All data must be stored securely using encryption standards (e.g., passwords hashed) |
| NFR05 | System uptime must be at least 99.5%                                                 |
| NFR06 | System must comply with data privacy regulations (e.g., GDPR)                        |
| NFR07 | Pages must load in under 3 seconds on average (performance)                          |
| NFR08 | System must be usable on major browsers (Chrome, Firefox, Safari, Edge)              |
| NFR09 | Must be built using maintainable and modular codebase (support future upgrades)      |
| NFR10 | System must log errors and support monitoring tools (e.g., Sentry, LogRocket)        |

---

## 📘 Suggested Learning Milestones:

### 📍 Before Phase 1:

* Basic Python: loops, functions, classes
* File I/O: reading/writing JSON or CSV
* Basic CLI programs
* Unit testing with `unittest`

### 📍 Before Phase 2:

* Django basics: project/app structure
* Models, views, templates (MVT pattern)
* Django ORM and migrations
* Forms and model forms
* Django Admin
* Authentication and user management
