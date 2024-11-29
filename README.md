 # Role-Based-Access-Control-System

see live on - https://role-based-access-control-system.onrender.com

Role-Based Access Control (RBAC) System
This project implements a robust Role-Based Access Control (RBAC) system, focusing on secure user authentication, authorization, and role management. The system is backend-focused, designed to ensure users can access features and resources according to their assigned roles (Admin, Moderator, or User).

# Features
1. User Authentication
User Registration: Allows users to sign up by providing a username, password, and selecting a role (User, Moderator, Admin).
User Login: Secure login functionality using JWT (JSON Web Tokens) to authenticate users.
2. Role-Based Authorization
Each role has specific access privileges to protected resources:
Admin: Full access to administrative dashboards and high-level system controls.
Moderator: Access to moderation features and specific resources.
User: Standard access to basic user functionalities.
Protected routes ensure only authorized users can access endpoints based on their roles.
3. Session Management
JWT-based authentication for maintaining user sessions securely.
Logout functionality invalidates tokens, ensuring secure session termination.
4. Modular and Scalable Architecture
Modularized backend structure for easy scalability and maintenance.
Separation of concerns for authentication, authorization, and resource management.
5. Test Endpoints
Endpoints for testing the role-based access control functionality:
User Profile: Accessible to all logged-in users.
Moderator Dashboard: Restricted to moderators and above.
Admin Dashboard: Restricted to admins.


# Key Highlights
Flask as Backend Framework:

Lightweight and modular, providing a clean API for managing routes and middleware.
Simplified user-role mapping and database interactions.
JWT-Based Security:

JSON Web Tokens are used to secure API endpoints, allowing stateless authentication.
Scalable and Modular Design:

Each role's functionality is separated into dedicated modules for better maintainability.
Custom Error Handling:

Unified response structure for errors and successful operations.
Usage
Register as a user, moderator, or admin using the /auth/register endpoint or UI form.
Login to receive an authentication token.
Use the token in the Authorization header (Bearer <token>) for accessing secured endpoints.

## Prerequisites

### System Requirements
- Python 3.x
- Pip (Python's package installer)

### Setup Steps
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/Ashishgupta291/Role-Based-Access-Control-System.git
    cd Role-Based-Access-Control-System
    ```

2. **Create a Virtual Environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use venv\Scripts\activate
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set Up the Database**:
    Using Flask-Migrate or manually:
    ```bash
    flask db init
    flask db migrate
    flask db upgrade
    ```

---

## Configuration

The project uses a configuration file (`config.py`) to manage application settings such as the secret key for JWT. 

Set the following environment variables:

- `FLASK_APP=app.py`
- `FLASK_ENV=development`
- `SECRET_KEY=your_secret_key` (Change to a secure key)

---

## Usage

### Running the Application
To start the Flask application, run:
```bash
python app.py
