The Charity Management System is a web-based platform developed for Charities to streamline their charitable activities and improve their organizational processes. The system aims to provide efficient management and organization of data related to people in need and the services provided by the charity.

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

## Notes:

- You must create a .env (environment variables) for the project to work. You should create it in the **Charity-Managment-Website/django_project**. It should include the following:
  - DEBUG = True
  - SECRET_KEY = {{your secret key}}
  - DATABASE_URL=sqlite:///db.sqlite3
  - EMAIL_HOST_PASSWORD = {{your sendgrid API}}
  - DEFAULT_FROM_EMAIL ={{your email}}
- The SECRET_KEY can be genereted using:
  ```
  python -c "import secrets;
  print(secrets.token_urlsafe())"
  ```
- The Email configuration can be found through using [SendGrid](https://app.sendgrid.com/), or any other email service provider. This is for the **forget password** functionality.

# Technologies

- Python (11.3.1)
- Django (4.0.10)
- SQLite3
- HTML, CSS, JS
- Bootstrap
- ChartJS
