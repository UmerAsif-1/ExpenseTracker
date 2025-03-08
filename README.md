# Expense Tracker

Expense Tracker is a web application built with Flask that allows users to track their expenses. Users can register, log in, and manage their expenses by adding, viewing, and deleting expense records.

## Features

- User registration and authentication
- Add new expenses with description and amount
- View and manage a list of expenses
- Delete expenses
- Responsive design with Bootstrap

## Requirements

- Python 3.7+
- PostgreSQL
- Flask
- Flask-SQLAlchemy
- Flask-Migrate
- Flask-Login
- Psycopg2-binary
- Python-dotenv

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/expense-tracker.git
    cd expense-tracker
    ```

2. **Create a virtual environment**:
    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment**:
    - On Windows:
        ```bash
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        source venv/bin/activate
        ```

4. **Install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

5. **Set up environment variables**:
    Create a `.env` file in the root directory and add the following:
    ````plaintext name=.env
    SECRET_KEY=your_secret_key
    DATABASE_URL=postgresql://yourusername:yourpassword@localhost/expense_tracker
    ````

6. **Initialize the database**:
    ```bash
    flask db init
    flask db migrate -m "Initial migration"
    flask db upgrade
    ```

7. **Run the application**:
    ```bash
    flask run
    ```

## Usage

1. **Register**:
    - Go to `http://127.0.0.1:5000/register` to create a new account.

2. **Log in**:
    - Go to `http://127.0.0.1:5000/login` to log into your account.

3. **Add Expense**:
    - Once logged in, go to `Add Expense` to add a new expense record.

4. **View Expenses**:
    - Your expenses will be listed on the home page.

5. **Delete Expense**:
    - You can delete any expense by clicking the 'Delete' button next to the expense.

