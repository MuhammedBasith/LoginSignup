# Login and Signup System with OTP

[![GitHub stars](https://img.shields.io/github/stars/MuhammedBasith/LoginSignup?style=for-the-badge)](https://github.com/MuhammedBasith/LoginSignup/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/MuhammedBasith/LoginSignup?style=for-the-badge)](https://github.com/MuhammedBasith/LoginSignup/network/members)
[![GitHub issues](https://img.shields.io/github/issues/MuhammedBasith/LoginSignup?style=for-the-badge)](https://github.com/MuhammedBasith/LoginSignup/issues)

A versatile command-line login and signup system implemented in Python, featuring OTP (One-Time Password) generation and email delivery.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Exit Codes](#exit-codes)
- [Contributing](#contributing)
- [License](#license)

## About

The Login and Signup System provides a straightforward command-line interface (CLI) for user authentication, registration, and login. It also includes a built-in OTP generation and email delivery feature, allowing you to easily integrate OTP-based authentication into your Python applications.

## Features

- User registration with email and password.
- Secure password hashing using bcrypt.
- User login and session management.
- OTP generation and email delivery for enhanced security.
- Minimalistic CLI interface for easy integration.
- Customizable to fit your project's needs.

## Getting Started

To get started with this login and signup system, follow these steps:

1. Clone the repository:

   ```sh
   git clone https://github.com/MuhammedBasith/LoginSignup.git
   ```

2. Navigate to the project directory:

   ```sh
   cd LoginSignup
   ```

3. Run the system:

   ```sh
   python main.py
   ```

4. Follow the on-screen instructions to register a user account, log in, and utilize the OTP functionality.

## Usage

The system provides a basic CLI for user registration and login. You can integrate it into your Python applications by importing the necessary functions and classes from the code.

Here's a simplified example of how to use the system in your Python script:

```python
from login_signup import UserManager

# Create a UserManager instance
user_manager = UserManager()

# Register a new user
user_manager.register_user("example@email.com", "password123")

# Login a user
user = user_manager.login("example@email.com", "password123")

if user:
    print("Login successful!")
else:
    print("Invalid email or password.")
```

Feel free to customize and extend the code to suit your specific project requirements.


## Exit Codes

The `main.py` script may return the following exit codes:

- `0`: No error.
- `1`: Successful operation.
- `2`: Invalid input.
- `4`: First user, file not found.

These exit codes can help you identify the status of the script's execution.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow our [Contributing Guidelines](CONTRIBUTING.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Thank you for using the Login and Signup System with OTP. We hope it simplifies user authentication and enhances security in your Python projects!
