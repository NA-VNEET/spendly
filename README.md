# Spendly - Personal Expense Tracker

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![Framework](https://img.shields.io/badge/flask-latest-lightgrey)

Spendly is a lightweight, intuitive personal finance and expense tracking application running on Flask. It helps users seamlessly log expenses, spot spending patterns, and stay on budget without the headache of complex spreadsheets. 

## ✨ Features

- **Quick Logging**: Add any expense in seconds with category, amount, date, and descriptions.
- **Pattern Recognition**: Interactive dashboards and category breakdowns (Vanilla JS) to understand your spending visually.
- **Budget Tracking**: Monitor remaining balances and track spending against monthly limits.
- **Custom Time Periods**: Filter data logically (e.g., this week, this month, or a custom range).
- **Responsive Design**: Fast and fully mobile-responsive UI created with semantic HTML and custom CSS. 
- **No-JS-Framework Setup**: Developed to be incredibly fast leveraging Vanilla JavaScript and pure CSS—no heavy frontend frameworks required.

## 🛠️ Tech Stack

- **Backend**: Python 3, Flask, Jinja2
- **Frontend**: HTML5, CSS3 (Custom Design System, CSS Variables), Vanilla JavaScript
- **Server**: WSGI-compatible setup (Ready for Gunicorn/Waitress)

## 📁 Project Structure

```text
expense-tracker/
├── app.py                  # Main Flask application and route definitions
├── static/
│   ├── css/
│   │   ├── style.css       # Global design system, variables, and UI components
│   │   └── landing.css     # Modular styles specific to the landing page
│   └── js/
│       └── main.js         # Frontend interactions and DOM manipulation
└── templates/
    ├── base.html           # Main Jinja layout wrapper
    ├── landing.html        # Public facing home page
    ├── login.html          # User authentication (Sign in)
    ├── register.html       # User authentication (Sign up)
    ├── privacy.html        # Privacy Policy page
    └── terms.html          # Terms and Conditions page
```

## 🚀 Getting Started

### Prerequisites

- [Python 3.8+](https://www.python.org/downloads/)
- `pip` (Python package installer)
- Git

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/expense-tracker.git
   cd expense-tracker
   ```

2. **Create and activate a virtual environment:**
   ```bash
   # On macOS/Linux
   python3 -m venv venv
   source venv/bin/activate

   # On Windows
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install Flask
   # If a requirements.txt exists: pip install -r requirements.txt
   ```

4. **Run the development server:**
   ```bash
   python3 app.py
   # Or using Flask CLI:
   # export FLASK_APP=app.py
   # export FLASK_ENV=development
   # flask run
   ```

5. **Access the application:**
   Open your browser and navigate to `http://127.0.0.1:5000` (or `http://127.0.0.1:5001` depending on port availability).

## 🔒 Security & Best Practices

- Wait to deploy until you swap the built-in Flask development server for a production-ready WSGI server like **Gunicorn** or **uWSGI**.
- Ensure to manage environment variables safely (e.g., `FLASK_SECRET_KEY`, Database URIs) using `.env` files in production environments via `python-dotenv`.

## 🤝 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


