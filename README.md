# 🛡️ LLM Guardrails Workshop

A Python-based LLM application that demonstrates how **input and output guardrails** can be used to make AI applications safer, more controlled, and reliable.

The project integrates the **Google Gemini API** with a web application and applies validation before and after the LLM generates a response.

---

## 📌 Project Overview

Large Language Models can sometimes generate inappropriate, unsafe, or unexpected responses.

This project demonstrates a simple guardrail architecture:

- Validate the user's input before sending it to the LLM.
- Send valid input to the Gemini model.
- Validate the generated response.
- Return the approved response to the user.

This approach helps create a more controlled LLM application.

---

## ✨ Key Features

- 🤖 Google Gemini API integration
- 🛡️ Input guardrails
- 🔍 Output guardrails
- 🌐 Web-based user interface
- 🐍 Python backend
- 🔐 Secure API-key management using environment variables
- 📦 Python virtual-environment support
- 🔄 Structured LLM request/response workflow

---

## 🏗️ Architecture

```text
                    ┌─────────────────┐
                    │      User       │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │  Web Interface  │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Input Guardrails│
                    └────────┬────────┘
                             │
                       Valid Input
                             │
                             ▼
                    ┌─────────────────┐
                    │   Gemini LLM    │
                    └────────┬────────┘
                             │
                       LLM Response
                             │
                             ▼
                    ┌─────────────────┐
                    │Output Guardrails│
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Safe Response   │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │      User       │
                    └─────────────────┘

## 🔄 Application Flow

User Input
    ↓
Input Validation
    ↓
Input Guardrails
    ↓
Gemini API
    ↓
Generated Response
    ↓
Output Guardrails
    ↓
Final Response

## 📁 Project Structure

LLM--GAUARDRAILS-WORKSHOP/
│
├── app.py
├── config.py
├── gemini_service.py
├── guardrails.py
├── output_guardrails.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── static/
│   ├── script.js
│   └── style.css
│
└── templates/
    └── index.html

## ⚙️ Installation

1. Clone the repository
git clone https://github.com/GaddeRamesh5236/LLM--GAUARDRAILS-WORKSHOP.git

2. Open the project
cd LLM--GAUARDRAILS-WORKSHOP

3. Create a virtual environment
python -m venv myvenv

4. Activate the virtual environment
Windows PowerShell
.\myvenv\Scripts\Activate.ps1

5. Install dependencies
pip install -r requirements.txt

## 🔑 Environment Configuration

Create a .env file in the project root.

GEMINI_API_KEY=your_gemini_api_key_here
GEMINI_MODEL=gemini-3.5-flash

## ▶️ Run the Application

Start the application:

python app.py

For example:

http://127.0.0.1:5000

## 🧪 Example Workflow
User Input
Hello, explain machine learning.
Processing
User Input
    ↓
Input Guardrail
    ↓
Gemini API
    ↓
Output Guardrail
    ↓
Response
Result

The application returns the validated LLM response through the web interface.

## 🎯 Learning Objectives

This project helped demonstrate:

Understanding of LLM application architecture
Integration of an external LLM API
Input validation
Output validation
Guardrail concepts
Environment-variable management
Flask application development
Frontend and backend integration
Git version control
GitHub project management

## 🚀 Future Improvements

Possible future enhancements include:

Prompt-injection detection
PII detection
Toxicity detection
Advanced content filtering
Better error handling
Logging and monitoring
Automated testing
Authentication
Cloud deployment
Docker containerization
