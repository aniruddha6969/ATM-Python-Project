ATM System - Simultaneous Python Project
Overview
This ATM system is a simulated Python project that mimics a simple banking interface. It allows users to log in, view their bank statement, withdraw and deposit money, change their PIN, and quit. The system is designed for multiple users, each with a separate account and PIN. Users can perform different operations like checking the balance, withdrawing cash (in multiples of 10), lodging money, and changing their PIN after successful login.

Features
User Authentication: Login using a username and PIN, with up to 3 attempts for entering the correct PIN.

Account Information: View the balance of the account after successful login.

Withdrawal: Withdraw money in multiples of 10 Euros, ensuring there are sufficient funds in the account.

Lodgement: Deposit money in multiples of 10 Euros.

Change PIN: Change the PIN after confirming the new one.

Quit: Exit the ATM system.

Requirements
Python 3.x (No additional libraries are required)

How to Use
Run the Script:

Simply run the script in any Python environment or terminal.

bash
Copy
Edit
python atm_simulation.py
Login:

Enter one of the predefined usernames (user, user2, user3).

Enter the correct PIN to proceed. You have 3 attempts to get the PIN correct.

Main Menu:

After logging in successfully, you will be presented with a menu with the following options:

Statement (S): View your current account balance.

Withdraw (W): Withdraw a specific amount, ensuring it is in multiples of 10.

Lodgement (L): Deposit money into your account, ensuring the amount is in multiples of 10.

Change PIN (P): Change your PIN after confirming the new one.

Quit (Q): Exit the system.

Pin Validation:

After 3 incorrect PIN attempts, your account will be locked.

ATM Simulation:

The system allows you to interact with it by typing the corresponding letter of the action you want to perform.

End Session:

You can end the session by typing Q (Quit).

Code Structure
Variables:
users: A list of usernames.

pins: A list of corresponding PINs for each user.

amounts: A list of account balances corresponding to each user.

Functions:
Login: Verifies the username and checks the PIN.

Withdraw: Validates the amount and updates the balance if valid.

Lodgement: Validates the amount and updates the balance if valid.

Change PIN: Allows the user to change their PIN after confirming the new one.

Example
bash
Copy
Edit
ENTER USER NAME: user
PLEASE ENTER PIN: ****
LOGIN SUCCESSFUL, CONTINUE
SELECT FROM FOLLOWING OPTIONS:
Statement__(S)
Withdraw___(W)
Lodgement__(L)
Change PIN_(P)
Quit_______(Q)
: s
user YOU HAVE 1000 EURO ON YOUR ACCOUNT.
Error Handling
Invalid Username: If the entered username does not exist in the list, the system will prompt the user to enter a valid username.

Invalid PIN: If the PIN entered is incorrect, the user will be given three attempts to input the correct PIN.

Invalid Amount: When withdrawing or depositing money, the amount must be a multiple of 10. If not, an error message will appear.

Contribution
Feel free to fork this project and make improvements. If you would like to contribute, please submit a pull request with your changes. If you find any issues or bugs, open an issue to report it.

License
This project is licensed under the MIT License - see the LICENSE file for details.
