The Charity Management System is an online platform designed to help charities enhance their charitable operations and optimize their administrative workflows. It's focused on effectively managing and organizing information concerning individuals in need and the support services offered by the charity.

## Features

- User registration and authentication: Charity organizers can create user accounts with unique credentials to access the system.
- Cases' records storage and management: The system allows researchers to input and update data about people in need, including their conditions and assistance provided.
- Charity locations management: Organizers can manage and update information about different charity locations.
- Analysis and reporting: The system generates statistical reports and visualizations based on the collected data, providing valuable insights to aid decision-making.
- User interface management: Different user roles, such as researchers and supervisors, have specific permissions and access levels within the system.
- Translation: Translated interface for the users in both Arabic and English using Django's Rosetta.

# Installation and Usage

## Requiremnts:

- [Python](https://www.python.org/downloads/) (3.11.3 is preferred)

1. (Optional) Create and activate a virtual environment (recommended):
   3.1. Installation on Windows:
   ```
   python -m venv .venv
   .venv\Scripts\Activate.ps1
   ```
   3.2. Installation on Linux:
   ```
   python3 -m venv env
   source  env/bin/activate
   ```
2. Install Dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run database migrations:
   ```
   python manage.py makemigrations
   python manage.py migrate
   ```
4. Create a superuser (supervisor/admin)
   ```
   python manage.py createsuperuser
   ```
5. Start the development server
   ```
   python manage.py runserver
   ```
6. Access the application:
   The application should now be running locally. Open a web browser and navigate to the specified address (e.g., `http://localhost:8000`) to access the Charity Management System.

# Technologies

- Python (11.3.1)
- Django (4.0.10)
- SQLite3
- HTML, CSS, JS
- Bootstrap
- ChartJS
