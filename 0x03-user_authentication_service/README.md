# 0x03. User Authentication Service

## Project Overview

This project involves creating a user authentication service using Flask, SQLAlchemy, and bcrypt. The service will handle user registration, login, sessions, password reset, and user profiles. While the industry standard recommends using established authentication modules or frameworks, this project aims to provide a learning experience by building the mechanisms from scratch.

## Learning Objectives

By the end of this project, you should be able to:

- Declare API routes in a Flask app
- Handle form data, cookies, and HTTP status codes
- Implement secure user registration and authentication
- Manage user sessions and profile retrieval
- Hash and store user passwords securely using bcrypt
- Create, validate, and update reset tokens for password recovery

## Project Structure

The project contains the following components:

1. **user.py**: Defines the User model using SQLAlchemy.
2. **db.py**: Implements the DB class to manage the database interactions.
3. **auth.py**: Defines the Auth class responsible for user authentication and sessions.
4. **app.py**: Creates the Flask app, handles routes, and sets up the server.
5. **main.py**: Contains end-to-end integration tests using the requests module.

## Getting Started

1. Install the required dependencies using pip:
   ```bash
   pip3 install Flask SQLAlchemy bcrypt requests
   ```

2. Initialize the SQLite database by running the following commands:
    ```bash
    python3 -c "from db import DB; DB().init_db()"
    ```

3. Start the Flask server:
    ```bash
    python3 app.py
    ```

4. Run the integration tests in the main.py module:
    ```bash
    python3 main.py
    ```

## Project Tasks

The project is divided into several tasks, covering various aspects of user authentication and session management. Detailed task descriptions and corresponding files can be found in the project directory.

## Additional Notes

For each task, ensure that your code adheres to the given requirements, such as style, documentation, and testing.
Remember that this project's primary goal is to learn the principles of user authentication and session management, rather than building production-ready code.

## Acknowledgments

This project is inspired by real-world authentication systems and aims to provide hands-on experience with implementing user authentication and session management in a secure and controlled environment.
