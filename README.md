# Python-Flask-Postgres-CP3

A token-based Flask RESTful API that enables users to register, log in, and manage recipe categories and recipes. The backend uses PostgreSQL for data storage and supports full CRUD operations.

## Features

- ✅ User Registration & Authentication (Token-based)
- ✅ Create, View, Update, Delete Recipe Categories
- ✅ Create, View, Update, Delete Recipes in Each Category
- ✅ Secure Endpoints for Logged-in Users
- ✅ Unit Testing Included

## Technologies Used

- Python 3.x
- Flask
- PostgreSQL
- Flask-RESTful
- Flask-JWT-Extended
- SQLAlchemy
- pytest (for testing)

## Getting Started

### Prerequisites

- Python 3.6+
- PostgreSQL
- Virtualenv (recommended)

### Setup Instructions

```bash
# Clone the repo
git clone https://github.com/Briankiboi/Python-Flask-Postgres-CP3.git
cd Python-Flask-Postgres-CP3

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables (example)
cp .env.example .env
# Edit .env and add your DATABASE_URL and JWT_SECRET_KEY

# Run database migrations
python manage.py db init
python manage.py db migrate
python manage.py db upgrade

# Run the application
python run.py
