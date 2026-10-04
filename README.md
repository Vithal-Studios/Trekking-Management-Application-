# 🏔️ Trekking Management Application

A web-based **Trekking Management Application** designed to simplify the management of trekking activities, trekkers, bookings, staff, and administrative operations through a role-based platform.

The application provides separate functionality for **Administrators, Trek Staff, and Trekkers**, allowing trekking organizations to manage the complete trekking workflow from trek creation and availability to bookings and user management.

---

## 📌 Project Overview

Managing trekking activities can involve multiple tasks such as creating and managing treks, maintaining trek availability, handling bookings, managing staff, and supporting trekkers.

This application provides a centralized platform to manage these activities efficiently.

### Core Workflow

```text
Admin / Staff Management
        ↓
Create & Manage Treks
        ↓
Trekkers Browse Available Treks
        ↓
Book Trek
        ↓
Manage Booking
        ↓
Track Trek & User Information
```

---

## ✨ Key Features

### 🔐 Authentication & Authorization
- User login and authentication
- Session-based authentication
- Role-based access control
- Secure password handling
- CSRF protection
- Separate access for Admin, Staff, and Trekker users

### 🏔️ Trek Management
- Create and manage trekking activities
- View trek details
- Manage trek status
- Manage trek availability and slots
- Update trek information
- Delete trekking activities
- Search and filter trekking information

### 🎟️ Booking Management
- Create trek bookings
- View booking details
- View booking history
- Manage booking status
- Cancel bookings
- Admin/Staff booking management

### 👥 User Management
- User registration and login
- View user profiles
- Manage user information
- Admin user management
- User activation/deactivation

### 👨‍💼 Staff Management
- Manage trekking staff
- Assign staff to trekking activities
- Staff-specific dashboard and operations
- Manage assigned trek information

### 📊 Dashboard & Analytics
- Dashboard views for different user roles
- Trek and booking statistics
- Chart-based data visualization

### 🔌 API Support
The application also provides API endpoints for:
- Treks
- Bookings
- Users

The API uses session-based authentication and supports operations such as GET, POST, PUT, and DELETE where applicable.

---

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| Backend | Python |
| Web Framework | Flask |
| Database | SQLAlchemy |
| Authentication | Flask-Login |
| Security / Forms | Flask-WTF |
| Password Hashing | bcrypt |
| Frontend | HTML, CSS, Jinja2 |
| API | Flask-based REST endpoints |

The project's current dependency list includes Flask, SQLAlchemy, Flask-Login, Flask-WTF, and bcrypt.

---

## 📂 Project Structure

```text
Trekking-Management-Application-
│
├── trek_management/
│   │
│   ├── app/
│   │   ├── routes/
│   │   ├── models/
│   │   └── ...
│   │
│   ├── scripts/
│   │
│   ├── static/
│   │
│   ├── templates/
│   │
│   ├── main.py
│   ├── requirements.txt
│   ├── API_SAMPLES.md
│   └── test_app.py
│
├── .gitignore
└── README.md
```

> The structure above represents the major application components; additional modules may be present inside the `app` and `scripts` directories.

---

## 🚀 Getting Started

### Prerequisites

Make sure the following are installed:

- Python 3.10+
- Git
- pip

### 1. Clone the Repository

```bash
git clone https://github.com/Vithal-Studios/Trekking-Management-Application-.git
```

### 2. Navigate to the Application

```bash
cd Trekking-Management-Application-/trek_management
```

### 3. Create a Virtual Environment

Windows:

```powershell
python -m venv venv
```

Activate it:

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
python main.py
```

The application runs locally on:

```text
http://127.0.0.1:5000
```

Open the URL in your web browser.

---

## 🔑 User Roles

### Administrator

Administrators have access to system-level management functionality such as:

- Trek management
- User management
- Staff management
- Booking management
- Administrative dashboards
- System-level operations

### Trek Staff

Staff members can manage trekking activities assigned to them and work with trek-related information and participants.

### Trekker

Trekkers can interact with available trekking activities, make bookings, view their booking information, and manage their profile.

---

## 🔌 API

The application provides API endpoints for managing core resources.

### Available API Resources

```text
/api/treks
/api/bookings
/api/users
```

Example:

```bash
curl -X GET "http://localhost:5000/api/treks?page=1&per_page=10&status=Open" \
     -b cookies.txt
```

The repository also contains `API_SAMPLES.md` with example API requests and responses.

---

## 🧪 Testing

The project includes:

```text
test_app.py
```

Tests can be executed using:

```bash
python -m unittest
```

or, depending on the project's test configuration:

```bash
python -m pytest
```

---

## 🔒 Security

The application includes several security-related mechanisms:

- Password hashing using bcrypt
- Session-based authentication
- Flask-Login authentication management
- CSRF protection
- HTTP-only session cookies
- SameSite cookie configuration
- Role-based authorization

---

## 🎯 Project Objectives

The main objectives of the Trekking Management Application are to:

- Centralize trekking activity management
- Simplify trek booking and tracking
- Provide role-specific functionality
- Improve administration of trekking operations
- Provide secure authentication and authorization
- Provide API access to core application resources
- Improve the overall experience for trekkers and staff

---

## 🔮 Future Enhancements

Potential future improvements include:

- Online payment integration
- Email and SMS notifications
- Real-time trek availability
- GPS and route tracking
- Interactive maps
- Weather information for trekking locations
- Mobile application
- Advanced analytics and reporting
- Automated booking reminders
- Cloud deployment

---

## 📄 License

This project is intended for educational and development purposes.

---

## 👨‍💻 Project

**Trekking Management Application**

Built with **Python, Flask, SQLAlchemy, HTML, CSS, and Jinja2**.
