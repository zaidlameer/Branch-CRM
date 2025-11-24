# Branch CRM

A centralized customer registration system designed to replace spreadsheet-based workflows across multiple branches. This project provides role-based access, unified customer data management, and a scalable architecture prepared for future expansion.

---

## Features

### User Authentication

* Secure sign-in and sign-out
* Role-based access control:

  * **Branch User**
  * **Head Office User**
  * **Administrator**
* User profile page

### Customer Management (CRUD)

* Create, read, update, and delete customers
* Soft delete implementation (customers marked inactive instead of removed)
* Sorting and listing with search filters
* Customer detail view
* Input validation and flash messages

---

## Tech Stack

### Backend

* **Django** (REST API)

### Frontend

* **React** (SPA)

### Database

* **PostgreSQL**

### Containerization

* **Docker** (for consistent local development)

### Deployment (previously hosted)

* **Microsoft Azure**

---

## Running Locally

### Requirements

* Docker & Docker Compose
  or
* Python 3.x, Node.js, PostgreSQL

### Using Docker (Recommended)

```bash
docker-compose up --build
```

Frontend: [http://localhost:3000](http://localhost:3000)
Backend API: [http://localhost:8000](http://localhost:8000)

---

## Environment Variables

Create `.env` files for both backend and frontend.

Backend example:

```
DATABASE_URL=postgres://user:password@db:5432/appdb
SECRET_KEY=your_django_secret
DEBUG=True
```

Frontend example:

```
REACT_APP_API_URL=http://localhost:8000
```

---

## Future Improvements

* Audit logging
* Branch-level dashboards
* Advanced analytics
* Customer notes and attachments
* Two-factor authentication

---

## License

This project is for educational use unless otherwise specified.
