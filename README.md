# URLSCOUTS
URLScourt uses explainable AI to detect phishing and malicious URLs, expose hidden threats, and protect people from online scams—turning every suspicious link into a smarter, safer click.
# 🔍 UrlScout — Smart URL Safety Checker

**Paste a link. We check it before you click it.**

UrlScout is a web-based cybersecurity project designed to help users identify potentially unsafe URLs before visiting them. It analyzes submitted links and provides a safety verdict to help users make informed decisions and avoid suspicious websites.

## 🚀 Features

* 🔗 **URL Analysis:** Submit a URL to check its potential safety.
* 🛡️ **Threat Detection:** Classifies URLs into categories such as Safe, Suspicious, or Malicious.
* 🔎 **Deep Scan:** Supports additional checks involving DNS records, SSL/TLS certificates, and redirects.
* 📊 **Risk Score:** Displays a score to help users understand the potential risk associated with a URL.
* 🕘 **Recent Checks:** Displays previously analyzed URLs and their results.
* ⚡ **Simple Interface:** Easy-to-use design for quick URL checking.

## 💡 Problem Statement

Malicious websites often use phishing links, deceptive domains, and suspicious redirects to trick users into revealing sensitive information or downloading harmful files.

Many users cannot easily determine whether a link is trustworthy before opening it.

UrlScout aims to simplify this process by providing a single interface for checking URLs and highlighting potential security risks.

## 🎯 Our Solution

UrlScout provides a convenient URL analysis interface that helps users assess suspicious links before visiting them.

Users can submit a URL, initiate an analysis, and review the resulting safety verdict and risk score. The deep-scan option is designed to provide additional information about DNS records, certificates, and redirects.

## 🛠️ Tech Stack

**Frontend**

* HTML5
* CSS3
* JavaScript

**Backend**

* Python
* Flask
* REST API

**Database**

* SQLite

**Security Analysis**

* DNS checks
* SSL/TLS certificate checks
* Redirect analysis

## ⚙️ How It Works

1. The user enters a URL into the UrlScout interface.
2. The frontend sends the URL to the Flask backend.
3. The backend performs the configured URL security checks.
4. The application evaluates the available results.
5. A verdict and risk score are returned to the frontend.
6. The result can appear in the recent-checks section.

## 📁 Project Structure

```text
URLScout/
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── scans.db
│
├── frontend/
│   ├── index.html
│   ├── script.js
│   └── style.css
│
└── README.md
```

*Note: Adjust the file names and folder structure above to match your actual repository.*

## 💻 Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/MinalKochrekar/URLScout.git
```

### 2. Navigate to the backend

```bash
cd URLScout/backend
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```powershell
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start the backend

```bash
python app.py
```

The Flask server should start at:

```text
http://127.0.0.1:5000
```

### 6. Open the frontend

Open `frontend/index.html` in you
