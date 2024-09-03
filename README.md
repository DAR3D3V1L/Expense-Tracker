# Expense Tracker

Expense Tracker is a web application built with Flask that allows users to track their expenses across various categories. It includes user authentication, the ability to add, update, delete expenses, and view them in a categorized list.

## Features

- User Registration and Authentication
- Add, Update, and Delete Expenses
- Categorize expenses (Food, Transport, Entertainment, etc.)
- View a summary of all expenses
- Responsive UI with Semantic UI

## Tech Stack

- **Backend**: Python, Flask, SQLAlchemy, Flask-Login
- **Frontend**: HTML, CSS, Semantic UI
- **Database**: SQLite
- **Deployment**: Docker

## Installation

### Prerequisites

- Python 3.9 or above
- Docker (for containerized deployment)

### Local Setup

1. **Clone the Repository**

   ```bash
   https://github.com/DAR3D3V1L/Expense-Tracker.git
   cd Expense-Tracker
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up the Database**

   Initialize the database and create tables.

   ```bash
   flask db upgrade
   ```

5. **Run the Application**

   Start the Flask application.

   ```bash
   flask run
   ```

   The application will be available at `http://127.0.0.1:5000`.

### Docker Setup

To run the application using Docker:

1. **Build the Docker Image**

   ```bash
   docker build -t Expense-Tracker .
   ```

2. **Run the Docker Container**

   ```bash
   docker run -p 8000:8000 Expense-Tracker
   ```

   The application will be available at `http://localhost:8000`.

## Usage

1. **Register a New User**: Open the app in your browser and go to the **Register** page. Fill in the registration form to create a new account.

2. **Login**: After registering, log in using your credentials.

3. **Add an Expense**: Navigate to the **Home** page and fill in the form to add a new expense.

4. **Update or Delete an Expense**: Click the **Update** or **Delete** buttons next to each expense in the list to modify or remove them.

## Folder Structure

```plaintext
Expense-Tracker/
├── app.py                # Main application file
├── models.py             # Database models
├── forms.py              # Form classes using Flask-WTF
├── templates/            # HTML templates
│   ├── base.html         # Base template
│   ├── home.html         # Home page template
│   ├── login.html        # Login page template
│   ├── register.html     # Register page template
│   └── update.html       # Update expense template
├── static/               # Static files (CSS, JS, Images)
│   └── style.css         # Custom styles
├── requirements.txt      # Python dependencies
└── Dockerfile            # Docker configuration
```

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a new Pull Request.

## Contact

For questions or support, please contact [devansh_arya@outlook.com].
