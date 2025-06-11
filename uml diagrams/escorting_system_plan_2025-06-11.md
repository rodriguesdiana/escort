# Escorting System Project Plan

## 📌 Project Overview

An escorting system where you can be either an **Escort** or a **Contractor**.

- **Escort:** Offers services, divided into three tiers:
  - Tier 1: Companion only
  - Tier 2: Play only
  - Tier 3: Game Night (Companion + Play)

- **Contractor:** Can search for and hire escorts.

---

## 🚧 Development Phases

### 🧱 Phase 1 – Terminal-Based CRUD in Python
- Learn Python OOP principles
- Build a CLI-based application
- Focus on logic, persistence, and input handling

### 🌐 Phase 2 – Django Web App + Deployment

#### Phase 2A – Django Development
- Learn Django framework, models, views, templates
- Implement same features from Phase 1 in web format

#### Phase 2B – Local Server Deployment
- Learn Apache/Nginx, systemd, local DNS via `/etc/hosts`
- Simulate production environment

---

## ✅ Functional Requirements

| # Cod | Requirement                                 |
|------|----------------------------------------------|
| FR01 | Must have a register of contractors          |
| FR02 | Must have a register of escorts              |
| FR03 | Escorts must have service tiers              |
| FR04 | Contractors must be able to search escorts   |
| FR05 | Booking system between contractors/escorts   |
| FR06 | Escorts can accept or reject bookings        |
| FR07 | Booking history viewable for both roles      |
| FR08 | Escorts can update their tier or availability|
| FR09 | Basic CLI interaction (Phase 1)              |
| FR10 | Admin panel in Django (Phase 2)              |

---

## 🛠️ Non-Functional Requirements

### General

| # Cod | Requirement                                          |
|------|-------------------------------------------------------|
| NFR01| Web application (Django)                              |
| NFR02| Code should be modular and readable                   |
| NFR03| Must be documented for personal learning              |
| NFR04| Use version control (e.g., Git)                       |

### Deployment-Specific

| # Cod | Requirement                                          |
|------|-------------------------------------------------------|
| NFR11| Must be deployable on a local Linux server            |
| NFR12| Use Apache or Nginx as a web server                   |
| NFR13| Set up local DNS via `/etc/hosts` (e.g., escort.test)|
| NFR14| Use systemd to run Django app as a service            |
| NFR15| Configure firewall to allow/deny ports                |
| NFR16| Use HTTPS with self-signed SSL                        |
| NFR17| Use BIND or simulate DNS manually (optional)          |
| NFR18| Log access/errors via Apache/Nginx                    |
| NFR19| Make accessible on local network                      |
| NFR20| Use PostgreSQL for production (optional)              |

---

## ⏳ Project Timeline Estimate (1 Day/Week)

| Phase | Duration       |
|-------|----------------|
| Phase 1 – Terminal CRUD | 4–5 weeks        |
| Phase 2A – Django Dev   | 6–8 weeks        |
| Phase 2B – Deployment   | 2–3 weeks        |
| **Total**               | **12–16 weeks**  |

---

## 🧠 Consistency Strategy

- Use **micro-tasks** per session (see below)
- Maintain a simple **learning log**
- Use weekly **retrospective** to reflect
- Focus on visible, small wins
- Optional: use Goblin Tools or physical task board

---

## 📘 Learning Log Template (Repeat Weekly)

```markdown
# Week X – Date

## 🎯 Focus
(e.g., Class design for Escort and Contractor)

## ✅ What I Did
- 
- 

## 😕 What Confused Me
- 

## 💡 One Thing I Learned
- 

## 🚀 Next Micro-Task
- 
```

---

## 🔧 First 6 Weekly Micro-Tasks

### Week 1 – Kickoff + Class Skeletons

- [ ] Create `User` base class with `name`, `id`
- [ ] Create `Escort` and `Contractor` subclasses
- [ ] Add `service_tier` attribute to `Escort`
- [ ] Print a list of sample escorts and their tiers

---

### Week 2 – Service Tier and CLI Menu

- [ ] Create `ServiceTier` enum
- [ ] Update `Escort` to use enum
- [ ] Build basic CLI menu to:
  - [ ] Add new escort
  - [ ] List all escorts

---

### Week 3 – Contractors + Booking (Draft)

- [ ] Create list of `Contractor` instances
- [ ] Add method for contractor to book an escort
- [ ] Print booking summary

---

### Week 4 – File Persistence

- [ ] Save escorts/contractors to file (JSON or `pickle`)
- [ ] Load data on startup
- [ ] Confirm persistence works correctly

---

### Week 5 – Error Handling + Search

- [ ] Add input validation (e.g., tier input must be valid)
- [ ] Filter escorts by tier
- [ ] Add try/except around main input loop

---

### Week 6 – Code Review + Modularization

- [ ] Split files into `main.py`, `models.py`, etc.
- [ ] Refactor CLI into functions
- [ ] Optional: Add unit test for `Escort`
- [ ] Write full learning log review for Phase 1

---

