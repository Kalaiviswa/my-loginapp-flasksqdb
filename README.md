# Flask Web Application

## Project Overview
A simple Flask web application built with SQLAlchemy to manage a user database. It provides RESTful API endpoints for user registration, login, and profile management. This project serves as a foundation for more advanced web application development.

---

## Features
- User registration and authentication.
- Integration with SQLite database using SQLAlchemy.
- RESTful API for managing user data.
- Modular project structure for scalability.

---

## Installation

### Prerequisites
- Python 3.8 or higher.
- Git installed on your system.

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set environment variables:**
   Create a `.env` file in the project root and add your Flask app configurations:
   ```env
   FLASK_APP=app.py
   FLASK_ENV=development
   SECRET_KEY=your_secret_key
   ```

5. **Initialize the database:**
   ```bash
   flask db init
   flask db migrate
   flask db upgrade
   ```

6. **Run the application:**
   ```bash
   flask run
   ```
   Access the application at `http://127.0.0.1:5000`.

---

## Usage
- **Registration Endpoint:**
  ```http
  POST /register
  ```
- **Login Endpoint:**
  ```http
  POST /login
  ```
- **User Profile Management:**
  ```http
  GET /profile
  ```

---

## Project Structure
```
project-root/
|-- app/
|   |-- __init__.py
|   |-- models.py
|   |-- routes.py
|-- migrations/
|-- templates/
|-- static/
|-- requirements.txt
|-- .env
|-- app.py
|-- README.md
|-- LICENSE
```

---

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

---

## Acknowledgments
- Flask: https://flask.palletsprojects.com/
- SQLAlchemy: https://www.sqlalchemy.org/

