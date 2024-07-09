useReducer Bank Account Application
Project Overview
This project is a simple bank account application built with React. It demonstrates the use of the useReducer hook to manage state and handle various account actions like opening an account, making deposits, withdrawals, requesting a loan, paying off a loan, and closing the account. The application also features basic styling to enhance the user experience.

Table of Contents
Installation
Usage
Components
State Management
Styling
License
Installation
To get started with this project, follow these steps:

Clone the repository:

sh
Copy code
git clone <repository-url>
Navigate to the project directory:

sh
Copy code
cd <project-directory>
Install dependencies:

sh
Copy code
npm install
Start the development server:

sh
Copy code
npm start
The application should now be running at http://localhost:3000.

Usage
To use the application:

Open your browser and navigate to http://localhost:3000.
You can open an account, deposit money, withdraw money, request a loan, pay off the loan, and close the account using the provided buttons.
Components
The application consists of the following main components:

App: The main component that renders the application and manages state using the useReducer hook.
reducer: A function to handle the state transitions based on the dispatched actions.
State Management
The application uses the useReducer hook for state management. The state consists of the following properties:

balance: The current balance of the account.
loan: The current loan amount.
isActive: A boolean indicating whether the account is active.
Reducer Actions
openAccount: Opens the account with an initial balance of 500 and sets isActive to true.
deposit: Increases the balance by the specified amount.
withdraw: Decreases the balance by the specified amount.
requestLoan: Requests a loan and adds the loan amount to the balance if no loan is currently active.
payLoan: Pays off the loan by deducting the loan amount from the balance.
closeAccount: Closes the account if there is no outstanding loan and the balance is zero.