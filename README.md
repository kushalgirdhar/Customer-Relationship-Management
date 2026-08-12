# Customer Relationship Management System (Django-CRM)

[![Python 3.12+](https://img.shields.io/badge/python-3.12%2B-blue.svg)](https://www.python.org/)
[![Django 6.0+](https://img.shields.io/badge/django-6.0%2B-green.svg)](https://www.djangoproject.com/)
[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL%203.0-orange.svg)](LICENSE)

An open-source, full-featured **Customer Relationship Management (CRM)** system built with **Python & Django**. Designed for businesses, agencies, and teams that need a unified solution for lead management, sales pipelines, task tracking, email marketing, and analytics.

---

## 🌟 Core Features

| 💼 Sales & CRM | 📋 Tasks & Projects | 📊 Analytics & Reports | ✉️ Email & Marketing |
|---|---|---|---|
| • Lead & Inquiry Tracking | • Project & Subtask Management | • Sales Funnel Reports | • Mass Email Campaigns |
| • Deal Pipeline Forecasting | • Office Memos to Tasks | • Income Summaries | • SMTP / IMAP Email Sync |
| • Companies & Contact Directory | • Internal Chat & File Sharing | • Lead Source Tracking | • Dynamic Email Templates |
| • Products & Invoice Payments | • Reminders & Tagging | • Conversion Statistics | • Automatic Contact Linkage |

---

## 🚀 Quick Start Guide

### 1. Prerequisites
- Python 3.12 or higher
- Git

### 2. Clone Repository
```bash
git clone https://github.com/kushalgirdhar/Customer-Relationship-Management.git
cd Customer-Relationship-Management
```

### 3. Create & Activate Virtual Environment
- **Windows**:
  ```cmd
  python -m venv myenv
  myenv\Scripts\activate
  ```
- **macOS / Linux**:
  ```bash
  python3 -m venv myenv
  source myenv/bin/activate
  ```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Initialize Database & Demo Data
Run `setupdata` to perform database migrations, load default fixtures (currencies, countries, departments), and generate default user credentials:
```bash
python manage.py setupdata
```

> **Note**: Upon completion, credentials for **SUPERUSER** and **SALES MANAGER** will be generated in your terminal output.

### 6. Run the Development Server
```bash
python manage.py runserver
```

---

## 🔑 Access Endpoints & Default Roles

| Interface | URL | Access Level | Description |
|---|---|---|---|
| **CRM Sales Dashboard** | `http://127.0.0.1:8000/en/123/` | Sales Manager & Team | Main operational CRM interface for managing leads, deals, tasks, and communications. |
| **System Admin Portal** | `http://127.0.0.1:8000/en/456-admin/` | Superuser / Admin | System administration portal for managing user permissions, groups, departments, and models. |

---

## ⚙️ Key Enhancements & Customized Features

- **Seamless Superuser Navigation**: Superusers can switch effortlessly between the CRM Sales Dashboard and System Admin Portal via top-navigation links.
- **Smart Middleware Authentication**: Unauthenticated users visiting `/en/456-admin/` are directed to the Admin Login screen.
- **SQLite Out-of-the-Box**: Configured for local development with zero external database dependencies needed for evaluation.

---

## 🛠️ Technology Stack

- **Backend**: Python, Django 6.0+
- **Database**: SQLite (Development) / PostgreSQL & MySQL supported (Production)
- **Frontend**: HTML5, CSS3, JavaScript, Django Admin Design System
- **Localization**: Supports 20+ interface languages with time zone aware settings.

---

## 📄 License

This project is licensed under the **AGPL-3.0 License**. See the [LICENSE](LICENSE) file for details.
