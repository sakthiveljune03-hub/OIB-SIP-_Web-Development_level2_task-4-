# Web Development Authentication System

A simple authentication system built with HTML, CSS, and JavaScript using browser localStorage for credential management.

## Project Overview

This project implements a basic user registration and login system with a secure page that displays personalized content for authenticated users.

## Features

- **User Registration**: New users can create an account with a username and password
- **User Login**: Existing users can authenticate with their credentials
- **Session Management**: Users remain logged in using localStorage
- **Secure Page**: Protected page that only authenticated users can access
- **Logout Functionality**: Users can securely log out and clear their session

## Project Structure

```
├── register.html      # User registration page
├── login page.html    # User login page
├── secure.html        # Protected page for authenticated users
└── README.md          # Project documentation
```

## File Descriptions

### register.html
- Allows new users to create an account
- Validates that both username and password fields are filled
- Stores credentials in browser localStorage
- Redirects to login page after successful registration

### login page.html
- Allows existing users to log in with their credentials
- Validates username and password against stored data
- Sets a session indicator in localStorage upon successful login
- Redirects to secure page for authenticated users

### secure.html
- Protected page that displays personalized welcome message
- Checks if user is authenticated; redirects to login if not
- Shows the logged-in username
- Provides logout functionality to end the user session

## How to Use

1. **Register a New Account**
   - Open `register.html` in your browser
   - Enter a username and password
   - Click "Register"
   - You will be redirected to the login page

2. **Login**
   - Enter your registered username and password
   - Click "Login"
   - Upon successful authentication, you'll be taken to the secure page

3. **Access Secure Page**
   - Only authenticated users can view this page
   - The page displays your username
   - Click "Logout" to end your session

4. **Logout**
   - Click the "Logout" button on the secure page
   - You'll be returned to the login page

## Technical Details

### Technologies Used
- **HTML5**: Page structure and layout
- **JavaScript**: Authentication logic and page interactions
- **Browser localStorage**: Client-side data storage for credentials

### Key Functions

**register.html**
- `register()`: Validates input, stores credentials, and redirects to login

**login page.html**
- `login()`: Authenticates user against stored credentials

**secure.html**
- `logout()`: Clears session and redirects to login

## Security Considerations

⚠️ **Important**: This is a demonstration project and should NOT be used in production. The following security measures are NOT implemented:

- Passwords are stored in plain text in localStorage
- No encryption or hashing is applied
- localStorage is vulnerable to XSS attacks
- No HTTPS/SSL security
- No server-side validation
- No protection against brute force attacks

For production applications, always use:
- Secure backend authentication (Node.js, Python, etc.)
- Password hashing (bcrypt, scrypt, Argon2)
- Secure sessions/JWT tokens
- HTTPS encryption
- Database storage (PostgreSQL, MongoDB, etc.)
- Server-side validation and security measures

## Getting Started

1. Download or clone the files
2. Open `register.html` in your web browser
3. Create a test account
4. Log in with your credentials
5. Explore the secure page



## Future Enhancements

- Add form validation (email format, password strength)
- Implement password confirmation field
- Add user profile page
- Add password reset functionality
- Add email verification
- Implement server-side backend
- Add database integration



## License

This project is provided as-is for educational purposes.