****Banking-System Project****

This is a simple Banking System developed in Python that includes a variety of essential features for managing bank accounts. The system allows users to deposit and withdraw money, open and close fixed deposits, check balances, and more. The project uses the getpass library to securely handle passwords.

**Features**
The banking system includes the following functionalities:

**Account Creation**: Create a new bank account.

**Deposit Money**: Deposit money into the user’s account.

**Withdraw Money**: Withdraw money from the user’s account.
**Fixed Deposit (FD)**:

      Open a Fixed Deposit (FD).
      Close a Fixed Deposit (FD) and transfer the principal and interest to the main account.
**Balance Enquiry**: Check the current balance in the user’s account.

**Password Configurations** : A secure password system using the getpass library to avoid password visibility in the terminal.



**Getting Started :**


**Prerequisites :**

 **.** Python 3.x installed on your machine.
 
 **.** The getpass library is used in this project, which is part of Python's standard library, so no additional installation is required.

 
**Link For The Respository**
     
    https://github.com/Codenaman21/Banking_system.git
    
**Code Structure**

The project consists of the following core components:

**bankingsystem.py**: Main script containing the core banking functionalities.

**(.txt) files To Store Data**: A file to store user information such as account balance, fixed deposit details, etc. (this file is for simulation purposes and should not be used for real banking systems).

**Core Functions:**

   **Create Account**

     Prompts the user to create an account by setting a username and password using the getpass library.
     Account data is saved in a local file (accounts.txt).
     
   **Deposit Money**

     Allows the user to deposit a specific amount into their bank account.
     Updates the balance in the system.
     
   **Withdraw Money**

      Allows the user to withdraw a specific amount from their account, as long as there is sufficient balance.
      
   **Open Fixed Deposit**

       Allows the user to open a Fixed Deposit with a specified amount and tenure.
       The Fixed Deposit will earn interest and can be closed after the tenure ends.
       Fixed Deposits data is saved in a local file (fixed_deposits.txt).
       
   **Close Fixed Deposit**

      Allows the user to close an FD and transfer the principal and interest back to the main account.
      
   **Check Balance**

      Displays the current balance in the user's account, including the available balance and any fixed deposits.
      
   **Password Configuration**

      The user can set a password for their account, and it is validated using the getpass library to ensure that the password is not visible when typing.

**Code Analysis**
**Main Script** : bankingsystem.py

 The main logic is implemented in banking_system.py. Here's a breakdown of the key sections:

**User Authentication:**

The program first asks the user to log in by entering their username and password. It uses the getpass library to securely accept the password without displaying it on the screen.

**Account Management:**

The program allows users to perform actions like depositing money, withdrawing funds, and checking their balance. It checks for sufficient balance before allowing withdrawals and displays an error message if the user tries to withdraw more than their available balance.

**Fixed Deposit:**

Users can open a fixed deposit for a specified duration. The system calculates interest (using a simple formula or predefined rate) and allows the user to close the FD after the tenure ends. The FD amount, along with interest, is added to the main balance when closed.

**File Handling:**

User data is stored and retrieved from a text file (accounts.txt). This file includes the username, account balance, and FD details(fixed_deposits.txt) and SIP dtails (sip_investments.txt) . It simulates a persistent storage solution for the sake of this project.

**Contributing :**

Feel free to contribute to this project! You can do so by:

Forking the repository and submitting a pull request.
Reporting any bugs or issues you encounter.

**License**

This project is licensed under the MIT License - see the LICENSE file for details
