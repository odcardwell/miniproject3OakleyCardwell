# miniproject3OakleyCardwell

### INF601 Advanced Programming with Python
### Oakley Cardwell

## Project Description

This project is a Flask-based web application that allows users to register, log in, and create, edit, and delete blog posts. The application demonstrates fundamental web development concepts using Python and Flask, including user authentication, database interactions, and the use of templates and static files.

### Application Features

- **User Authentication**: Secure registration and login system using hashed passwords.
- **Create, Read, Update, Delete (CRUD) Operations**: Users can create new posts, view all posts, edit their own posts, and delete posts.
- **Database Integration**: Utilizes SQLite for data storage, with a `user` table and a `post` table linked via a foreign key.
- **Bootstrap Integration**: Enhanced user interface using Bootstrap components like modals and accordions for a responsive and modern design.
- **Session Management**: Securely manages user sessions to protect routes that require authentication.

### Understanding the Application

Upon launching the application, users can:

- **Register**: Create a new user account by providing a username and password.
- **Log In**: Access their account using their credentials.
- **View Posts**: See a list of all posts displayed in an accordion format.
- **Create Posts**: Authenticated users can create new posts with a title and body.
- **Edit Posts**: Users can edit posts that they have authored.
- **Delete Posts**: Users can delete their own posts, with a confirmation modal to prevent accidental deletions.

The application provides a simple yet powerful platform to demonstrate how a web application can manage user-generated content securely and efficiently.

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/odcardwell/miniproject3OakleyCardwell.git
   ```
   
2. **Navigate to the Project Directory**:

   ```bash
   cd miniproject3OakleyCardwell
   ```
3. **Create a Virtual Environment**:
   ```bash
   cd miniproject3OakleyCardwell
   ```
   It's recommended to use a virtual environment to manage dependencies.


4. **Activate the Virtual Environment**:
   ```bash
   source venv\Scripts\activate
   ```
   
5. **Install the Required Dependencies**:
   ```bash
   pip install -r requirements.txt
    ```

## Database Initialization

Before running the application, you need to initialize the database.

1. **Set the Flask Application Environment Variable**:

   - On Windows (Command Prompt):

     ```bash
     set FLASK_APP=flaskr
     ```

   - On Windows (PowerShell):

     ```powershell
     $env:FLASK_APP = "flaskr"
     ```

   - On macOS/Linux:

     ```bash
     export FLASK_APP=flaskr
     ```

2. **Initialize the Database**:

   ```bash
   flask init-db

You should see the message: Initialized the database.

## Running the Development Server

1. **Set the Flask Environment to Development (Optional but Recommended)**:

   This enables debug mode, which provides detailed error messages.

   - On Windows (Command Prompt):

     ```bash
     set FLASK_ENV=development
     ```

   - On Windows (PowerShell):

     ```powershell
     $env:FLASK_ENV = "development"
     ```

   - On macOS/Linux:

     ```bash
     export FLASK_ENV=development
     ```

2. **Run the Flask Application**:

   ```bash
   flask run
   
  The application will start, and you'll see output similar to:
  
  ```bash
   * Serving Flask app 'flaskr'
   * Debug mode: on
  WARNING: This is a development server. Do not use it in a production deployment.
   * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
   * Restarting with stat
   * Debugger is active!
   * Debugger PIN: 123-456-789
   ```

3. **Access the Application**:

   Open a web browser and navigate to `http://127.0.0.1:5000/` to view the application.

## Usage

1. **Register a New User**:

   - Click on the "Register" link in the navigation bar.
   - Fill out the registration form with a username and password.

2. **Log In**:

   - After registering, you can log in using the "Login" link.
   - Enter your credentials to access your account.

3. **Create a New Post**:

   - Once logged in, click on "Create a new post".
   - Fill in the title and body of your post and submit.

4. **View Posts**:

   - Posts are displayed on the home page in an accordion format.
   - Click on a post title to expand and view its content.

5. **Edit or Delete a Post**:

   - If you are the author of a post, you will see "Edit" and "Delete" options.
   - Click "Edit" to modify your post.
   - Click "Delete" to remove your post; a confirmation modal will appear.

6. **Log Out**:

   - Use the "Logout" link in the navigation bar to end your session.

## Requirements

### requirements.txt

Ensure that the following packages are listed in your `requirements.txt` file:

- click==8.0.1 
- Flask==2.0.1 
- itsdangerous==2.0.1 
- Jinja2==3.0.1 
- MarkupSafe==2.0.1 
- Werkzeug==2.0.1

You can generate this file by running:

```bash
pip freeze > requirements.txt
```


## Notes

- **Security Considerations**:

  - The `SECRET_KEY` in the application should be changed to a random value in a production environment.
  - Passwords are securely hashed using Werkzeug's security utilities.

- **Development vs. Production**:

  - This application is intended for educational purposes and runs in development mode.
  - For production deployment, additional configuration and security measures are required.

## Conclusion

This project serves as a practical demonstration of building a web application with Flask, covering key concepts like user authentication, database interactions, and template rendering. By following the installation and usage instructions, you can explore and extend the application to suit your learning objectives.

---
