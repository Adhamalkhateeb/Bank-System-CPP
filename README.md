# 🏦 Banking System in C++

A console-based banking system built using C++ with file handling. This project allows you to manage client accounts with functionalities such as adding, deleting, updating, and searching clients. It also supports transactions like deposits and withdrawals.

## 📦 Features

### Client Management
- ✅ **Add New Clients:** Create new client accounts with unique account numbers.
- ✅ **Delete Clients:** Remove client data securely.
- ✅ **Update Client Information:** Modify existing client details.
- ✅ **View All Clients:** Display all registered clients in a tabular format.
- ✅ **Search Clients:** Find clients using their account number.

### Transactions
- 💰 **Deposit Money:** Add funds to a client's account.
- 💸 **Withdraw Money:** Deduct funds from a client's account (with balance validation).
- 📊 **Show Total Balances:** Display the total balance of all clients.

### User Management (New!)
- 👤 **Add New Users:** Create new users with unique usernames.
- 🗑️ **Delete Users:** Remove users securely (admin users cannot be deleted).
- 🔄 **Update User Information:** Modify user details and permissions.
- 🔍 **Find Users:** Search for users by username.

### Permissions System (New!)
- 🔐 **Role-Based Access Control:** Restrict access to features based on user permissions.
- 🛡️ **Admin Privileges:** Admin users have full access to all features.

### Login System (New!)
- 🔑 **Secure Authentication:** Users must log in with a username and password.
- 🚪 **Logout:** Log out and return to the login screen.

## 📁 Project Structure

* ├── 📄 Bank Last edition.cpp # Main source code file
* ├── 📄 Clients.txt # Data file storing client information
* ├── 📄 Users.txt # Data file storing user information (New!)
* ├── 📄 README.md # Project documentation
* ├── 📄 CHANGELOG.md # Track changes to the project (New!)
* └── 📄 .gitignore # Specifies files to ignore in Git (New!)

## 🛠️ Technologies Used

- **Programming Language:** C++
- **File Handling:** `fstream` for persistent data storage.
- **Standard Library:** `vector`, `string`, `iomanip`
- **Permissions System:** Bitwise operations for role-based access control.

## 🚀 Getting Started

### Prerequisites
- A C++ compiler (e.g., g++).
- Git (optional, for cloning the repository).

### Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/BankingSystemCPP.git
   cd BankingSystemCPP
   ```
2. **Compile the Code:**
   ```bash
    g++ main.cpp -o BankingSystem
   ```
3.  **Run the Program:**
   ```bash
   ./BankingSystem
   ```
4.  **Log in:**
   ```bash   
    Username: Admin
    Password: 1234
   ```
   
## 📖 Usage Guide
### Main Menu Options:
1. Show All Clients: Display a list of all clients.

2. Add New Client: Create a new client account.

3. Delete Client: Remove a client account.

4. Update Client Information: Modify client details.

5. Find Client: Search for a client by account number.

6. Transactions: Access the transactions menu (deposit, withdraw, show total balances).

7. Manage Users (New!): Access the user management menu (add, delete, update, find users).

8. Logout (New!): Log out and return to the login screen.

### Transactions Menu:
1. Deposit: Add funds to a client's account.

2. Withdraw: Deduct funds from a client's account (with balance validation).

3. Show Total Balances: Display the total balance of all clients.

### User Management Menu (New!):
1. List Users: Display all users.

2. Add New User: Create a new user.

3. Delete User: Remove a user (admin users cannot be deleted).

4. Update User: Modify user details and permissions.

5. Find User: Search for a user by username.

   
## 📁 Data Handling:

### Client Data (Clients.txt)
* Format: Each client record is stored in a single line with fields separated by #//#.

* Fields: AccountNumber#//#PinCode#//#Name#//#Phone#//#Balance

* Example:
  - 12345#//#6789#//#John Doe#//#123-456-7890#//#1000
  - 67890#//#1234#//#Jane Smith#//#987-654-3210#//#2000

### User Data (Users.txt)
* Format: Each user record is stored in a single line with fields separated by #//#.

* Fields: Username#//#Password#//#Permissions

* Example:
   - Admin#//#1234#//#-1
   - User1#//#password1#//#15
   - User2#//#password2#//#31

## Permissions
### Permissions are stored as integers using bitwise flags:

1: List Clients

2: Add New Client

4: Delete Client

8: Update Client

16: Find Client

32: Transactions

64: Manage Users

-1: Full Access (Admin)

## 🤝 Contributing

Contributions are welcome!Feel free to fork the repository and submit a pull request.

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## ⭐️ If you like this project, consider giving it a star on GitHub! ⭐️
