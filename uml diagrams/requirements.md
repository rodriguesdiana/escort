## 🧱 **Phase 1: Terminal-Based CRUD (Python + OOP Focus)**

**Goal:** Learn Python syntax, object-oriented design, and basic data handling.

### ✅ Functional Requirements for Phase 1

| # Cod | Requirement                                                                              |
| ----- | ---------------------------------------------------------------------------------------- |
| FR01  | Mantain contractors (name, password)                                                     |
| FR02  | Mantain escorts (name, password, tier)                                                   |
| FR03  | Escorts can accept/reject a booking (simulate manually)                                  |
| FR04  | Must allow escorts to define and update their service tier                               |
| FR05  | Must allow a contractor to view available escorts by tier                                |
| FR06  | Allow booking simulation (contractor books escort)                                       |
| FR07  | Use basic file I/O or in-memory storage (e.g., list/dict) to persist data during runtime |
| FR08  | Simulate a basic login/authentication flow using usernames/passwords                     |
| FR09  | List current and past bookings in terminal interface                                     |

### ✅ Non-Functional Requirements for Phase 1

| # Cod | Requirement                                                         |
| ----- | ------------------------------------------------------------------- |
| NFR01 | Code must follow object-oriented principles (use classes)           |
| NFR02 | Code must be organized into modules (e.g., models, services, utils) |
| NFR03 | Use command-line interface (CLI) menus for interaction              |
| NFR04 | Should include exception handling for input validation              |
| NFR05 | Code should be documented (docstrings + comments)                   |
| NFR06 | Write unit tests for major classes/methods (using `unittest`)       |
| NFR07 | Store data in **persistent local files** (e.g., JSON or CSV)        |

---

## 🌐 **Phase 2: Django Web Application**

**Goal:** Learn Django framework, MVC pattern, models/forms/views/templates, web dev practices.

### ✅ Functional Requirements for Phase 2

| # Cod | Requirement                                                                          |
| ----- | --------------------------------------------------------------------------------     |
| FR01  | User registration and login (escorts and contractors) using Django’s auth system     |
| FR02  | Escorts can create/edit/delete service offerings (CRUD)                              |
| FR03  | Contractors can browse escorts and filter by service tier                            |
| FR04  | Contractors can request/book a service                                               |
| FR05  | Escorts can approve/reject bookings via dashboard                                    |
| FR06  | User profiles with photos, bio, and contact preferences                              |
| FR07  | *Optional*: Basic messaging/chat between users (or Django notifications)             |
| FR08  | Contractor can rate escort after the appointment                                     |
| FR09  | Escort can rate contractor after the appointment                                     |
| FR10  | Admin dashboard to moderate users/services                                           |
| FR11  | *Optional*: Add payment simulation or Stripe integration (for learning)              |
| FR12  | Implement booking logic with proper models and relational DB (PostgreSQL or SQLite)  |
| FR13  | Booking calendar/schedule overview                                                   |

### ✅ Non-Functional Requirements for Phase 2

| # Cod | Requirement                                                                            |
| ----- | -------------------------------------------------------------------------------------- |
| NFR01 | Web app should follow Django’s MVC architecture                                        |
| NFR02 | Use responsive templates with Bootstrap or Tailwind                                    |
| NFR03 | Use Django ORM for database interaction                                                |
| NFR04 | Secure authentication (Django auth, password hashing)                                  |
| NFR05 | Form validation with Django Forms                                                      |
| NFR06 | Store data in a relational DB (SQLite/PostgreSQL)                                      |
| NFR07 | Modular and reusable apps (Django app structure)                                       |
| NFR08 | Follow good project structure, version control with Git                                |
| NFR09 | Basic logging and error handling                                                       |
| NFR10 | *Optional*: Deploy to a free hosting service (e.g., PythonAnywhere, Vercel for Django) |
| NFR08 | Write basic unit tests for views, models, and forms                                    |
| NFR09 | Add logging and error messages for debugging                                           |
| NFR10 | Document your project with README and setup instructions                               |

### 🎓 Learning Tips

* **Phase 1:** Focus on class design (Escort, Contractor, Service), polymorphism (service tiers), and data structures.
* **Phase 2:** Explore Django’s admin panel, URL routing, views, templates, and models. Slowly integrate Django-specific features like `signals`, `middleware`, or `custom managers`.

---

## ✅ Add These Requirements to Support Server and Infrastructure Learning

### 🔧 **New Non-Functional Requirements for Phase 2 (Deployment Focus)**

| # Cod | Requirement                                                                                   |
| ----- | --------------------------------------------------------------------------------------------- |
| NFR11 | The application must be deployable on a local Linux server                                    |
| NFR12 | Must configure Apache or Nginx to serve the Django project via WSGI or ASGI                   |
| NFR13 | Must configure a custom domain in `/etc/hosts` for local DNS simulation (e.g., `escort.test`) |
| NFR14 | Must use systemd to run the Django server as a background service                             |
| NFR15 | Must understand and apply basic firewall rules (e.g., `ufw`) to open/close ports              |
| NFR16 | Must support HTTPS via self-signed certificate (SSL/TLS basics)                               |
| NFR17 | Should simulate basic DNS resolution using BIND or `/etc/hosts`                               |
| NFR18 | Should log server access and errors using Apache/Nginx logs                                   |
| NFR19 | Should be accessible via local network (e.g., another device on same LAN)                     |
| NFR20 | Optional: Set up PostgreSQL and configure Django to use it on your local server               |

---

### 🧱 Your Updated Development Phases (Now with Infra Learning)

#### 🌐 **Phase 2 (Web App + Deployment)**

You now have *two sub-phases*:

* **2A: Django App Development** – You build and test locally using `runserver`.
* **2B: Local Server Deployment** – You set up Apache/Nginx, local DNS, and systemd service to simulate a production server.

---

### 🗂️ Tools and Concepts You'll Touch

| Category           | Tools/Concepts                                        |
| ------------------ | ----------------------------------------------------- |
| Web Server         | Apache, Nginx, WSGI (Gunicorn/uWSGI)                  |
| DNS                | `/etc/hosts`, optionally BIND for full DNS simulation |
| Networking         | TCP/IP ports, `netstat`, `ufw`, localhost, loopback   |
| Process Management | `systemctl`, `journalctl`, creating services          |
| Security           | HTTPS, SSL certs, basic Linux permissions             |
| Databases          | PostgreSQL or SQLite migrations on production         |
| Logs               | Apache/Nginx logs, Django logs                        |

---

### ✨ Bonus Functional Requirement (Optional)

| # Cod | Requirement                                                                                          |
| ----- | ---------------------------------------------------------------------------------------------------- |
| FR11  | Admin panel accessible only through a secure path (e.g., `/admin123`) to simulate security practices |

---
### Links

- [Timeline](timeline.md)
- [Milestones](gr.md)
- [Project Plan](escorting_system_plan_2025-06-11.md)