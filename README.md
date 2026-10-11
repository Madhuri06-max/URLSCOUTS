# 🔍 URLSCOUTS — AI-Powered URL Safety Checker

**Check before you click. Stay safe online.**

URLSCOUTS is a web-based URL security analysis tool designed to help users identify potentially malicious, suspicious, and phishing URLs before visiting them. It analyzes URL characteristics, evaluates security-related signals, and presents an explainable verdict with a risk score to help users make more informed decisions online.

## ✨ Features

- 🔗 **URL Analysis:** Submit a URL for security analysis.
- 🛡️ **Threat Detection:** Identify suspicious URL patterns and potential phishing indicators.
- 🧠 **Explainable Analysis:** Provide understandable reasons behind detected risk signals.
- 📊 **Risk Scoring:** Display a score representing the assessed risk of a URL.
- 🌐 **Deep Scan:** Perform additional checks involving DNS, SSL/TLS certificates, and redirects when enabled.
- 🕘 **Scan History:** Store and retrieve recent URL analysis results using SQLite.
- ⚡ **Web Interface:** A simple interface built with HTML, CSS, and JavaScript.
- 🔌 **REST API:** Use Flask endpoints to communicate between the frontend and backend.

## 🎯 Problem Statement

Phishing websites and malicious links often imitate legitimate services to trick users into sharing passwords, financial information, or other sensitive data.

URLSCOUTS aims to make URL security analysis more accessible by highlighting suspicious characteristics and providing understandable risk indicators before users visit a link.

## 💡 Our Solution

URLSCOUTS combines URL-based analysis with configurable security checks to assess potentially unsafe links. It returns a verdict, a risk score, and analysis results through a web interface.

The project focuses on making URL analysis easier to understand by presenting the signals that contribute to an assessment rather than relying only on a simple safe-or-unsafe label.

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Python, Flask |
| API | Flask REST endpoints |
| Database | SQLite |
| HTTP Requests | Requests |
| Cross-Origin Support | Flask-CORS |
| Security Checks | URL analysis, DNS, SSL/TLS, redirects |

## 🏗️ Project Structure

```text
URLSCOUTS/
├── backend/
├── frontend/
│   └── index.html
├── .vscode/
├── app.py
├── index.html
├── requirements.txt
├── README.md
└── scans.db
```

*Note: The structure above reflects the files identified during setup. The backend and frontend folders may contain additional files.*

## ⚙️ Getting Started

### Prerequisites

- Python 3.10 or a compatible version
- Git
- A modern web browser

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/URLSCOUTS.git
cd URLSCOUTS
```

Replace `YOUR-USERNAME` with the GitHub account that hosts the repository.

### 2. Create a virtual environment

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```powershell
python -m pip install -r requirements.txt
```

### 4. Start the application

```powershell
python app.py
```

### 5. Open URLSCOUTS

Visit the following address in your browser:

http://127.0.0.1:5000/

Keep the terminal open while using the application. Press `Ctrl + C` to stop the development server.

## 🔌 API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/` | Serve the web interface |
| GET | `/api/health` | Check API health |
| POST | `/api/analyze` | Analyze a submitted URL |
| GET | `/api/history` | Retrieve recent scan results |

### Example API Request

```http
POST /api/analyze
Content-Type: application/json
```

```json
{
  "url": "https://example.com",
  "deep": false
}
```

The analysis endpoint returns a JSON response containing the analysis results. The exact fields depend on the application's implementation.

## 🔒 Security Disclaimer

URLSCOUTS is an assistive security analysis tool, not a guarantee that a website is safe or malicious. A low-risk result does not guarantee safety, and a high-risk result does not by itself prove malicious intent.

Avoid entering sensitive personal information on unfamiliar websites. Use additional security checks when evaluating suspicious links.

## 🚧 Future Improvements

- Integrate reputable threat intelligence feeds.
- Improve phishing detection and classification.
- Enhance the user interface and accessibility.
- Add visual analytics and scan-history filtering.
- Expand automated testing and error handling.
- Improve deployment and security monitoring.

## 👥 Contributors

Developed collaboratively as a cybersecurity project focused on safer browsing and understandable URL risk analysis.

## ⭐ Support

If you find this project interesting, consider starring the repository on GitHub.

**URLSCOUTS — Check before you click.**
