# Flask Web App

This is a simple full-stack web application built using **Flask** on the backend and **HTML/CSS/JS** on the frontend. I followed along with [Tech With Tim’s tutorial](https://www.youtube.com/watch?v=dam0GPOAvVI) to understand how Flask apps are structured and deployed.

## 🔧 What it does

- Users can sign up, log in, and manage notes.
- Auth is handled securely using hashed passwords (Flask's built-in security practices).
- Logged-in users can add and delete notes from their account.
- Flash messages are used for feedback (e.g., invalid login, note deleted).
- Client-side logic is handled with a bit of vanilla JS for dynamic note deletion.

## 💡 Why I built this

I wanted to get more hands-on with Flask and see how a full-stack Python web app is put together. While I've worked with modern frameworks like React and Next.js, this helped me better understand backend flow, routing, templating (Jinja2), session handling, and form validation in a lightweight environment.

## 🛠️ Tech Stack

- **Python 3 / Flask** – Backend
- **SQLite** – Local development database
- **Jinja2** – Templating engine
- **HTML / CSS / JavaScript** – Frontend
- **Flask-Login** – User session management
- **Werkzeug** – Password hashing

## 📁 Project Structure (Simplified)

```html
/website
  /static
    index.js               # Handles frontend JS (delete note on click)
  /templates
    home.html
    login.html
    sign_up.html
  __init__.py              # App factory + route registration
  auth.py                  # Auth routes
  models.py                # DB models (User, Note)
  views.py                 # Main routes (home, add/delete note)
main.py                    # Entry point
```

## 📹 Demo

You can check out a quick demo on YouTube: [Flask App Demo](https://www.youtube.com/watch?v=dam0GPOAvVI)

## 📝 What I learned

- Structuring a Flask app using Blueprints
- Handling user auth securely with session cookies
- Creating a local database using SQLAlchemy
- Using form data and flash messages to improve UX
- How a basic frontend and backend communicate (through fetch and API calls)
