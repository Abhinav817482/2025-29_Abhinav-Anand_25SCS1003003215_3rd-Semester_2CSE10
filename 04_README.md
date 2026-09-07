# 🛡️ Cybersecurity Utility Tools

Four complementary cybersecurity utilities built during my internship — covering password security, network vulnerability scanning, ML-based phishing detection, and secure authentication.

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 📖 Overview

This repository brings together four independent, thematically connected cybersecurity tools, each addressing a different layer of information security:

| # | Tool | Addresses |
|---|------|-----------|
| 1 | 🔐 **Password Strength Evaluator** | Strength of individual user credentials |
| 2 | 🔍 **Vulnerability Scanner** | Security posture of a network / web app |
| 3 | 📧 **Phishing Email Detection Model** | Human-targeted phishing threats |
| 4 | 🔑 **Secure Login System** | Safeguarding the authentication process |

Built as part of a B.Tech CSE (AI/ML) internship, this project was an opportunity to apply cryptography, network scanning, machine learning, and secure web development in practice.

---

## ✨ Features

### 1. Password Strength Evaluator
- Checks length, character complexity (uppercase/lowercase/digits/symbols), and uniqueness
- Suggests stronger alternatives for weak passwords
- Optional database check to prevent reuse of old passwords

### 2. Vulnerability Scanner
- Scans a target host/network for open ports and weak configurations
- Detects outdated software versions via banner grabbing
- Generates a simple, readable vulnerability report

### 3. Phishing Email Detection Model
- Trained on a labelled dataset of phishing vs. legitimate emails
- Extracts features from email text and embedded URLs
- Classifies emails as **Phishing** or **Safe**
- Reports accuracy and a confusion matrix

### 4. Secure Login System
- User registration and login with salted password hashing (bcrypt / Argon2)
- Input validation and parameterised queries (SQL-injection safe)
- Session management with logout
- Optional Two-Factor Authentication (2FA)

---

## 🛠️ Tech Stack

| Module | Technologies |
|--------|-------------|
| Password Strength Evaluator | Python, `re`, zxcvbn / custom scoring logic, SQLite |
| Vulnerability Scanner | Python, `nmap` / `python-nmap`, sockets |
| Phishing Email Detection | Python, Scikit-learn, Pandas, NumPy, NLTK, TF-IDF, Matplotlib |
| Secure Login System | Python (Flask/Django) or Node.js, bcrypt/Argon2, HTML-CSS-JS, SQLite/MySQL |

---

## 📂 Project Structure

```
cybersecurity-utility-tools/
├── password-strength-evaluator/
│   ├── evaluator.py
│   └── requirements.txt
├── vulnerability-scanner/
│   ├── scanner.py
│   └── requirements.txt
├── phishing-email-detection/
│   ├── train_model.py
│   ├── dataset/
│   └── requirements.txt
├── secure-login-system/
│   ├── app.py
│   ├── templates/
│   └── requirements.txt
├── docs/
│   └── Internship_Report_Abhinav_Anand.docx
├── README.md
└── LICENSE
```

> Adjust the tree above to match your actual folder names once each module is in place.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- pip
- (Optional) `nmap` installed on your system for the Vulnerability Scanner

### Installation

```bash
git clone https://github.com/abhinav817482/cybersecurity-utility-tools.git
cd cybersecurity-utility-tools
pip install -r requirements.txt
```

### Running each module

```bash
# Password Strength Evaluator
python password-strength-evaluator/evaluator.py

# Vulnerability Scanner (only against systems you own or have permission to test)
python vulnerability-scanner/scanner.py --target <ip-or-hostname>

# Phishing Email Detection Model
python phishing-email-detection/train_model.py

# Secure Login System
python secure-login-system/app.py
```

---

## 📊 Results

- **Phishing Detection Model:** classifies emails as Phishing/Safe with accuracy and a confusion matrix reported after training (add your actual numbers here once available).
- **Vulnerability Scanner:** produces a summary report of open ports, weak configurations, and outdated services.

---

## ⚠️ Responsible Use

The Vulnerability Scanner is intended **only** for systems and networks you own or have explicit permission to test (e.g. local/lab environments). Do not scan systems without authorization.

---

## 🗺️ Roadmap

- [ ] Add GUI/web dashboard for the Vulnerability Scanner
- [ ] Expand phishing dataset and compare classifier models
- [ ] Add unit tests for each module
- [ ] Dockerize the Secure Login System

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Abhinav Anand**
B.Tech CSE (AI/ML), IILM University
GitHub: [@abhinav817482](https://github.com/abhinav817482)
