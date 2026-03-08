# PSUSphere

## Project Description

PSUSphere is a web application designed to help organizations within Palawan State University manage their student members. It provides a centralized system for tracking colleges, academic programs, student organizations, and memberships — all through a clean, dashboard-driven interface.

## Features

- **Dashboard Overview** — Live summary cards showing total students, organizations, programs, and students who joined in the current year.
- **Full CRUD Support** — Create, read, update, and delete records across all entities: Colleges, Programs, Organizations, Students, and Organization Members.
- **Search Functionality** — Search across all list views by relevant fields (e.g., student name, organization name, college, program).
- **Sorting** — Sort Organization Members by last name or date joined; sort Programs by name or college.
- **Pagination** — All list views are paginated for easier navigation of large datasets.
- **Admin Panel** — Enhanced Django admin interface with search, filtering, and display customization for all models.

## Data Models

| Model | Description |
|---|---|
| College | Top-level academic unit |
| Program | Academic program belonging to a college |
| Student | Student record linked to a program |
| Organization | Student org optionally linked to a college |
| OrgMember | Links a student to an organization with a date joined |

## Tech Stack

- **Backend:** Django 6.0.2 (Python)
- **Database:** SQLite
- **Frontend:** Bootstrap, jQuery, Chartist, Ready Admin Theme
- **Other:** django-widget-tweaks, Faker (for seed data)

## Installation

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Apply migrations:
   ```bash
   python manage.py migrate
   ```
4. (Optional) Load initial seed data:
   ```bash
   python manage.py create_initial_data
   ```
5. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Authors

**Allen Glenn Flojemon Fernandez**
allenglennfernandez04@gmail.com

**Eli Karl Torres Arnejo**
arnejoelikarl@gmail.com