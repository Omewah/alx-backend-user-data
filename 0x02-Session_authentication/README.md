
# 0x02 Session Authentication Project

**Project Description:**

This project aims to implement a Session Authentication mechanism in a Flask-based Python application. The project covers various tasks related to session management, user authentication, cookies, and more.

**Project Structure:**

The project is organized into several tasks, each building upon the previous ones. Here's a brief overview of the tasks:

1. **Et moi et moi et moi!**
   - Implements a basic authentication system for user endpoints.
   - Adds a new endpoint: GET `/users/me` to retrieve the authenticated User object.

2. **Empty session**
   - Introduces the concept of Session Authentication.
   - Creates a basic `SessionAuth` class to manage sessions.

3. **Create a session**
   - Enhances the `SessionAuth` class to generate and manage session IDs.
   - Allows creating session IDs for user authentication.

4. **Session cookie**
   - Adds a method to retrieve a session cookie from a request.
   - Demonstrates how to use session cookies for user identification.

5. **Before request**
   - Updates the authentication mechanism to exclude certain routes from authentication.
   - Handles authentication based on session cookies.

6. **Use Session ID for identifying a User**
   - Enhances the `SessionAuth` class to link session IDs with user IDs.
   - Demonstrates how to identify users using session IDs.

7. **New view for Session Authentication**
   - Creates a new Flask view for handling session authentication.
   - Implements a route for user login using session authentication.

8. **Logout**
   - Adds a route for user logout using session authentication.
   - Allows users to log out and end their session.

9. **Expiration? (Advanced)**
   - Introduces session expiration by creating a `SessionExpAuth` class.
   - Implements session expiration based on a defined duration.

10. **Sessions in database (Advanced)**
    - Implements a model for storing user sessions in a database.
    - Creates a `SessionDBAuth` class to handle session authentication using a database.

**Usage:**

1. Clone this repository:
   ```
   git clone <https://github.com/ThengweTheFirst/alx-backend-user-data.git>
   ```

2. Navigate to the project directory:
   ```
   cd 0x02-Session_authentication
   ```

3. Install project dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Set up environment variables (optional but recommended):
   - `API_HOST`: The host address for the API (default: `0.0.0.0`)
   - `API_PORT`: The port number for the API (default: `5000`)
   - `AUTH_TYPE`: Authentication type (`basic_auth`, `session_auth`, `session_exp_auth`, or `session_db_auth`)
   - `SESSION_NAME`: Name of the session cookie (default: `_my_session_id`)
   - `SESSION_DURATION`: Session duration in seconds (only for `session_exp_auth`)

5. Run the application:
   ```
   python -m api.v1.app
   ```

