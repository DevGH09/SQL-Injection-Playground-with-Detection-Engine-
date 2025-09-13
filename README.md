SQL Injection Playground with Detection Engine

A hands-on educational project designed to help users learn about SQL Injection (SQLi) vulnerabilities, their impact, and how to prevent them. This repository includes a vulnerable web application alongside a real-time detection engine that identifies SQLi attempts. It serves as a practical learning tool for cybersecurity enthusiasts, developers, and penetration testers.

📂 Project Structure

Vulnerable App – A deliberately insecure web application with common SQL injection flaws, built using PHP and SQLite (or Flask and SQLite depending on implementation).

Detection Engine – A Python-based tool that monitors traffic and detects suspicious SQL injection patterns in real time.

Documentation – Guides on how to run, test, and secure the vulnerable app.

✅ Features

Simulated SQL Injection Scenarios – Explore login and search forms with intentional vulnerabilities.

Real-time Attack Detection – The engine logs and analyzes abnormal requests, identifying attempts like tautologies, UNION attacks, and error-based injections.

Logging & Reporting – All injection attempts are recorded for further analysis.

Prevention Techniques – Demonstrates how parameterized queries and input sanitization can block attacks.

📌 Tech Stack

Frontend & Backend: PHP/Flask + SQLite

Detection Engine: Python (regex-based pattern matching and request monitoring)

Logging: Local file-based logs for audit and review

Security Concepts: SQL Injection types, parameterized queries, error handling

🚀 Getting Started
Prerequisites

Python 3.x

PHP or Flask environment

SQLite

requests Python library (pip install requests)

Installation

Clone this repository:

git clone https://github.com/DevGH09/SQL-Injection-Playground-with-Detection-Engine-


Set up the vulnerable application:

For PHP:

Place the files in your web server's root directory.

Start the server (php -S localhost:8000).

For Flask:

Install dependencies and run the app:

pip install -r requirements.txt
python app.py


Run the detection engine:

python detection_engine.py


Explore:

Access the vulnerable pages (e.g., http://localhost:8000/login.php).

Try different payloads and observe how the detection engine logs suspicious activities.

📖 How to Use

Test Vulnerabilities – Experiment with various SQL injection payloads to understand how attackers exploit web applications.

Monitor Attacks – Watch the detection engine output to learn how attack signatures are recognized.

Apply Fixes – Modify the vulnerable code to use prepared statements and proper validation to prevent attacks.

Analyze Logs – Review the logs for patterns and anomalies that indicate attempted attacks.

🔒 Security Lessons Covered

What SQL Injection is and how attackers exploit it.

Understanding tautology-based injections, UNION attacks, and error-based injections.

Importance of input validation and prepared statements.

Real-time monitoring and logging for cybersecurity defense.

📂 Future Improvements

Add support for more complex injection types.

Integrate with SIEM tools for centralized monitoring.

Implement machine learning-based anomaly detection.

Create a web dashboard for easier interaction and visualization.

📄 License

This project is licensed under the MIT License
