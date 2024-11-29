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
