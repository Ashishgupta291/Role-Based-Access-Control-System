# Role-Based-Access-Control-System

see live on - https://role-based-access-control-system.onrender.com

Role-Based Access Control (RBAC) System
This project implements a Role-Based Access Control (RBAC) System, providing a secure and user-friendly platform for managing users, their roles, and access to resources. The system is designed to simplify authentication and authorization tasks while maintaining a responsive and intuitive interface.

# Features
1. User Authentication
Secure login for existing users with token-based session management.
New user registration with role assignment options: User, Moderator, or Admin.
2. Role-Based Access
Different roles have access to distinct resources:
User Profile for general users.
Moderator Dashboard for moderators.
Admin Dashboard for administrators.
Resources are dynamically displayed based on user roles.
3. Dynamic Forms
Default Login Form: Users can log in directly.
Register Option: New users can toggle to the registration form and back to login.
4. Personalized Experience
Welcome message displaying the logged-in user's name.
Logout button positioned at the top-right corner for easy access.
5. Modern and Responsive UI
Built using HTML, CSS, and JavaScript.
Clean, responsive design with flexbox-based layouts for a seamless user experience across devices.
Technologies Used
HTML/CSS: For creating the structure and styling of the application.
JavaScript: For dynamic form handling and API integration.
Fetch API: For secure communication with backend endpoints.
Setup and Usage
1. Clone the Repository
bash
Copy code
git clone https://github.com/your-username/rbac-system.git
cd rbac-system
2. Backend API
Ensure the backend API endpoints for registration, login, resource fetching, and logout are running. You can use the following endpoints:

/auth/register - User registration.
/auth/login - User login.
/user/profile - User resources.
/moderator/moderator_dashboard - Moderator resources.
/admin/dashboard - Admin resources.
/auth/logout - Logout.
3. Run the Application
python app.py
