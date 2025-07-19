A Minimal Flask Website (Black & White Themed)

This is a **sample Flask web project** designed to demonstrate the basic structure of a Flask application using **template inheritance** and a clean **black & white theme**.
> ⚠️ **Note**: This is just a sample project and **not an actual business website**. It serves as a demonstration of how Flask can be used to build basic web pages with reusable components.

---

## 🚀 Project Overview
This project includes the following pages:
- **Home Page**
- **About Us Page**
- **Contact Page**

Each page uses a **common layout** (header/footer) thanks to **template inheritance** in Flask.

---

## 🧱 What is Template Inheritance?
Flask uses the Jinja2 templating engine, which supports template inheritance. That means we create a base template (like base.html) that includes parts that are common to all pages — such as:
- The HTML structure (`<head>`, `<body>`)
- Navigation bar
- Footer
In short, template inheritance means creating one common design layout and reusing it on every page by just changing the middle part (the content).
Then, each page like home.html, about.html, or contact.html only needs to fill in the content block like this:

```html
{% extends 'base.html' %}

{% block content %}
    <h1>Welcome to Home Page</h1>
{% endblock %}
```

📁 Project Structure:
```
FlaskSite/
│
├── static/
│   └── css/
│       └── styles.css         # Your black & white theme styles
│
├── templates/
│   ├── base.html              # Main layout template
│   ├── home.html              # Home page
│   ├── about.html             # About us page
│   └── contact.html           # Contact page
│
├── app.py                     # Flask app
```

⚙️ How to Run This Project
Make sure you have Python and Flask installed.

Step 1: Install Flask
pip install flask

Step 2: Run the App
python app.py
The app will start running at: http://127.0.0.1:5000/
