# Money Tracker 

This app was created as a capstone project for ADA Developers Academy. The purpose of this app is to easily visualize, in a simple way, how our money is distributed between our expenses, income, and savings. This visualization helps users make better financial decisions.

## Features

### Category Management

Manage your income and expenses by creating, updating, and deleting categories. Assign colors to categories for easy visual identification.

### Transaction Recording

Effortlessly record your financial transactions. Include details such as the transaction's name, amount, type (income, expense or savings). Categorize each transaction under the appropriate category.

### Data Visualization

Gain insights into your financial habits with an interactive pie chart. Visualize your spending and income patterns to understand where your money is being spent and how much you're saving.

### Transaction History

Keep track of all your financial activities. Access a comprehensive history of all recorded transactions, complete with important details like transaction description and amounts.

### Labeling and Filtering

Organize your transactions with ease. Attach labels or tags to transactions for simple categorization. 

### Slack Notifications

Receive real-time updates with Slack notifications for each posted transaction. Stay informed about your financial activities without having to constantly check the app.

## Dependencies 
Frontend
*React
Backend
*Express
*Node 
*MongoDB

## API Documentation

### Categories

#### Create a Category

- **Route:** `POST /categories`
- **Description:** Create a new category for income or expenses.
- **Request Body:** None
- **Response:** Returns the created category with type and color.

#### Get Categories

- **Route:** `GET /categories`
- **Description:** Get a list of all categories.
- **Response:** Returns an array of categories with type and color.

### Transactions

#### Create a Transaction

- **Route:** `POST /transaction`
- **Description:** Create a new transaction.
- **Request Body:** Include `name`, `type`, and `amount`.
- **Response:** Returns the created transaction with details.

#### Get Transactions

- **Route:** `GET /transaction`
- **Description:** Get a list of all transactions.
- **Response:** Returns an array of transactions.

#### Delete a Transaction

- **Route:** `DELETE /transaction`
- **Description:** Delete a transaction by providing the transaction details in the request body.
- **Request Body:** Include transaction details to delete.
- **Response:** Returns a message indicating whether the record was deleted or not.

### Labels

#### Get Transaction Labels with Colors

- **Route:** `GET /labels`
- **Description:** Get transaction labels along with their associated colors.
- **Response:** Returns an array of transaction details with labels and colors.

## Deployment

The Expense Tracker App has been deployed on [Render](https://render.com/).

You can access the deployed app at: [https://money-tracker-3k43.onrender.com/]

## Getting Started

1. Clone this repository.
2. Install dependencies using `npm install`.
3. Set up your MongoDB database connection.
4. Start the server using `npm start`.

---

Thank you for using the Money Tracker App! These features are designed to provide you with a comprehensive tool for managing your finances effectively and making informed financial decisions.
