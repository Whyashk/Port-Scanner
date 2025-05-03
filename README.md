# 🛡️ Port Scanner Web Application 🛡️

A lightweight, browser-based **port-scanning tool** that enables you to discover open TCP ports on any IPv4 address or domain name through an intuitive web interface. Built with **Python** and **Flask**, this project wraps a simple socket-based scanning engine in a responsive frontend, allowing users to input targets and port ranges without touching the command line. 🚀


---

📸 Screenshot

![App Screenshot](static/Screenshot.png)

---

## 📋 Table of Contents
1. [✨ Features](#-features)
2. [🧰 Tech Stack](#-tech-stack)
3. [🔧 Setup Instructions](#-setup-instructions)
4. [🚀 Usage](#-usage)
5. [📁 Project Structure](#-project-structure)
6. [🤝 Contributing](#-contributing)
7. [📄 License](#-license)

---

## ✨ Features

- 🔍 **Multi-Target Scanning**: Enter single or comma-separated targets (IP addresses or domains).
- 🎯 **Custom Port Ranges**: Specify any range (e.g., `1-1024`, `20-80`).
- ⚡ **Real-Time Feedback**: See open ports as they are discovered in a clean table.
- 🔒 **User Authentication**: Secure login/register system to protect access (optional module).
- 📱 **Responsive UI**: Designed with HTML5, CSS3, and JavaScript for seamless desktop and mobile use.
- 📂 **Modular Codebase**: Separate modules for scanning logic, routing, and templates for maintainability.

---

## 🧰 Tech Stack

- **Python 3.9+** — Core language for backend logic.
- **Flask** — Lightweight web framework for routing and API handling.
- **Socket** — Python standard library for TCP connect scans.
- **HTML5, CSS3, JS** — Frontend technologies for user interface.
- **Jinja2** — Flask’s templating engine.

---

## 🔧 Setup Instructions

Follow these steps to get the application running on your local machine:

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/Port-Scanner-Tool.git
   cd Port-Scanner-Tool
   ```

2. **Create & activate a virtual environment** (recommended)
   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # macOS/Linux
   source venv/bin/activate
   ```

3. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment variables** (optional)
   - Create a `.env` file at the project root.
   - Define `SECRET_KEY` for Flask session management:
     ```env
     SECRET_KEY=your_secret_key_here
     ```

5. **Run the application**
   ```bash
   python app.py
   ```

6. **Access the web interface**
   - Open your browser and visit `http://localhost:5000`


---

## 🚀 Usage

1. **Register or Log In** (if authentication is enabled).
2. **Enter target(s)** in the input field—you can use comma-separated lists.
3. **Specify port range** (e.g., `1-1000`).
4. **Click "Start Scan"** and watch the open ports populate the results table.
5. **Export results** as CSV (optional feature) or review them directly on your dashboard.

---

## 📁 Project Structure

```bash
Port-Scanner-Tool/
├── app.py               # Flask application entry point
├── scanner.py           # Core port scanning logic
├── requirements.txt     # Python dependencies
├── .env                 # Environment variables (SECRET_KEY)
├── LICENSE              # Apache 2.0 License
├── static/              # Static assets
│   ├── css/             # Stylesheets
│   ├── js/              # Client-side scripts
│   └── images/          # Screenshots and logos
└── templates/           # HTML templates (Jinja2)
    ├── base.html        # Base template layout
    ├── index.html       # Scan form and results
    └── auth.html        # Login/Register pages
```

---

## 🤝 Contributing

Contributions and improvements are welcome!
1. ⭐ Star the repo
2. 🍴 Fork the project
3. 📝 Create a feature branch (`git checkout -b feature-name`)
4. 🚀 Commit your changes (`git commit -m 'Add awesome feature'`)
5. 📬 Push to the branch (`git push origin feature-name`)
6. 🔀 Open a Pull Request

Please follow the existing code style and include clear, descriptive commit messages.

---

## 📄 License

This project is licensed under the **Apache 2.0 License**. See the [LICENSE](LICENSE) file for details.

---

✨ **Happy Scanning!** ✨

