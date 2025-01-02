# Online Banking System

## Overview

The Online Banking System is a simple console-based application that allows users to register, log in, check their balance, deposit and withdraw money, transfer funds to other users, and change their password. This system is designed for users to manage their bank accounts securely and efficiently through a simple interface.

## Features

- **User Registration**: Users can create an account with their phone number, account number, and password.
- **Login**: Registered users can log in using their phone number and password.
- **Balance Inquiry**: Users can check their current account balance.
- **Deposit Funds**: Users can deposit funds into their account.
- **Withdraw Funds**: Users can withdraw funds from their account with a condition that the withdrawal amount must be a multiple of 500.
- **Fund Transfer**: Users can transfer funds to another registered user.
- **Change Password**: Users can change their password securely.
- **Persistent Data Storage**: All user data is stored in a file based on the user's phone number (e.g., `phone.dat`) ensuring the data is persistent across sessions.

## Technologies Used

- **C Programming Language**: The system is implemented using the C programming language.
- **File Handling**: User data is stored in `.dat` files on the system using file handling operations (`fopen`, `fwrite`, `fread`).

## File Structure

The application uses the following file structure:
- **`filename.dat`**: A file created for each user where their account information is stored.
  - Contains the following data:
    - `phone`: User's phone number
    - `ac`: Account number
    - `password`: User's account password
    - `balance`: User's current account balance

## User Instructions

### Registration
1. When prompted, select option `1` to register a new account.
2. Enter your account number, phone number, and a new password.
3. The system will store your information in a file and register your account.

### Login
1. Select option `2` to log into your existing account.
2. Enter your registered phone number and password.
3. If the credentials are correct, the system will grant access to your account.

### Available Options After Login
Once logged in, you will have the following options:
- **Balance Inquiry**: Option `1` will display your current balance.
- **Deposit Funds**: Option `2` allows you to deposit money into your account.
- **Withdraw Funds**: Option `3` allows you to withdraw money from your account, with the condition that the amount is a multiple of 500.
- **Fund Transfer**: Option `4` allows you to transfer funds to another registered user.
- **Change Password**: Option `5` lets you change your password.

After completing any transaction, you will be asked whether you want to continue with further transactions.

### Exiting
Once you are finished, the system will automatically save your data, and you can safely exit.

## Limitations
- The system does not support any external databases; it uses file-based storage for user information.
- Withdrawals are only allowed in multiples of 500.
- Error handling is minimal, so make sure to input the correct values.

## Future Enhancements
- Integration with an actual database system (e.g., MySQL, SQLite) for more robust data management.
- A graphical user interface (GUI) for a better user experience.
- Implementation of additional security features like two-factor authentication.
- Support for different currencies and more complex banking features such as loan applications or bill payments.

## Acknowledgements
- C Programming Language for providing a foundation for developing this simple banking system.
