Backend – Application Flow & Functional Overview
1. Application Entry Point

When a client/customer accesses the website, they are first shown the Homepage.

The Homepage contains a “Sign In” button.
--------------------------------------------------------------------

2. Authentication Flow
Sign In

When the user clicks on the Sign In button, they are redirected to the Login Page.

If the user does not have an existing account, login will not proceed.

Instead, the system will prompt the user to Create Account.

Create Account

The Create Account page allows new users to register.

Once the account is successfully created:

The user is redirected back to the Login Page.

Login

After entering valid credentials:

The user is authenticated.

On successful login, the user is redirected to the User Dashboard.
------------------------------------------------------------------------------------------

3. User Dashboard & Role-Based Access

After login, the user lands on the User Dashboard.

Dashboard Dropdown Menu

The dashboard contains a dropdown menu, whose options depend on the user’s role.

Normal User

If the logged-in user has a USER role:

The dropdown menu shows:

User

Homepage

Admin User

If the logged-in user has an ADMIN role:

The dropdown menu shows:

User

Homepage

Admin Page
-----------------------------------------------------------------------

4. Admin Functionality

When an Admin clicks on the Admin Page option:

The application directly navigates to the Admin Dashboard/Page.

Any changes made on the Admin Page:

Are processed by the backend.

Are immediately reflected on the frontend.

This ensures real-time synchronization between admin operations and user-facing content.
------------------------------------------------------------------------------------------------------

5. Frontend–Backend Interaction

The frontend communicates with the backend APIs for:

Authentication (Login / Logout)

Role-based access control

Data updates made by the Admin

The system ensures:

Smooth navigation

Fast response

Seamless user experience
------------------------------------------------------------------------------------------
6. Logout

Logged-in users can log out at any time.

On logout:

The session/token is cleared.

The user is redirected back to the Homepage.
----------------------------------------------------------------------------------------------
7. Technology & Implementation Notes

Backend and frontend integration is designed to work smoothly and efficiently.

Authentication, authorization, and role handling are implemented using standard backend practices.

The implementation language/framework can be chosen based on developer preference.
