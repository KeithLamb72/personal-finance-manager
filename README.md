# Personal Finance Manager

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

Personal Finance Manager is a web application that allows users to manage their finances by tracking income, expenses, and savings. Users can visualize their financial data using charts and set financial goals to achieve better financial health.

## Features

- User authentication (register, login, logout)
- Add, edit, delete transactions (income and expenses)
- Categorize transactions
- Dashboard with financial data visualization (charts)
- Generate monthly and yearly financial reports
- Set and track financial goals

## Technologies

### Backend

- Node.js
- Express
- MongoDB
- JWT (JSON Web Tokens)
- Bcrypt.js

### Frontend

- React
- React Router
- Axios
- Chart.js
- React Chart.js 2

## Project Structure

### Backend

```
server/
│
├── config/
│   └── db.js
│
├── controllers/
│   ├── authController.js
│   └── financeController.js
│
├── models/
│   ├── User.js
│   └── Transaction.js
│
├── routes/
│   ├── authRoutes.js
│   └── financeRoutes.js
│
├── middleware/
│   └── authMiddleware.js
│
├── .env
├── server.js
└── package.json
```

### Frontend

```
client/
│
├── public/
│   └── index.html
│
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   │   ├── Login.js
│   │   │   ├── Register.js
│   │   │
│   │   ├── Finance/
│   │   │   ├── AddTransaction.js
│   │   │   ├── TransactionList.js
│   │   │   └── TransactionChart.js
│   │   │
│   │   ├── Layout/
│   │   │   ├── Header.js
│   │   │   ├── Footer.js
│   │   │
│   ├── pages/
│   │   ├── Home.js
│   │   ├── Dashboard.js
│   │   ├── Login.js
│   │   ├── Register.js
│   │
│   ├── App.js
│   ├── index.js
│
├── .env
├── package.json
└── README.md
```

## Setup and Installation

### Prerequisites

- Node.js (v14.x or higher)
- MongoDB

### Backend

1. Clone the repository and navigate to the `server` directory:

   ```bash
   git clone https://github.com/your-username/personal-finance-manager.git
   cd personal-finance-manager/server
   ```

2. Install backend dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the `server` directory and add your MongoDB URI and JWT secret:

   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

4. Start the backend server:

   ```bash
   node server.js
   ```

### Frontend

1. Navigate to the `client` directory:

   ```bash
   cd ../client
   ```

2. Install frontend dependencies:

   ```bash
   npm install
   ```

3. Start the React development server:

   ```bash
   npm start
   ```

4. Open your browser and go to `http://localhost:3000` to see the application.

## Usage

### Authentication

- Register a new user.
- Log in with the registered user credentials.
- The dashboard will be accessible upon successful login.

### Managing Transactions

- Add new income or expense transactions.
- Edit or delete existing transactions.
- Categorize transactions for better organization.

### Dashboard

- View an overview of your financial data.
- Visualize income and expenses using charts.
- Track financial goals.

## Endpoints

### Authentication

- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Log in an existing user.

### Transactions

- `POST /api/finance/transaction`: Add a new transaction.
- `GET /api/finance/transactions`: Get all transactions for the logged-in user.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes with clear and descriptive messages.
4. Push your changes to your fork.
5. Submit a pull request with a detailed description of your changes.

## Contact

For questions or suggestions, please contact:

- Keith Lamb: [keithianlamb@gmail.com](mailto:keithianlamb@gmail.com)
- GitHub: [Keith-Lamb](https://github.com/KeithLamb72)
