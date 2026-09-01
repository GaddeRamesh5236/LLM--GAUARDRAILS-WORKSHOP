# LLM--GAUARDRAILS-WORKSHOP

A practical project demonstrating how to build an LLM-powered application with input and output guardrails using Python and Google's Gemini API.

## 🚀 Project Overview

This project demonstrates how guardrails can be used to make Large Language Model (LLM) applications safer and more reliable.

The application processes user input through validation and guardrail checks before sending requests to the LLM. The generated response is then checked using output guardrails before being returned to the user.

## ✨ Features

- 🤖 Gemini API integration
- 🛡️ Input guardrails
- 🔍 Output guardrails
- 🚫 Prevents unsafe or inappropriate inputs
- ✅ Validates LLM-generated responses
- 🌐 Web-based user interface
- 🐍 Python backend
- 🔐 Environment variable support for API keys

## 🏗️ Project Structure

```text
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

## 🛠️ Technologies Used

Python
Google Gemini API
Flask
HTML
CSS
JavaScript
python-dotenv
LLM Guardrails


## 🔄 Application Flow

User Input
    ↓
Input Guardrails
    ↓
Gemini LLM
    ↓
Output Guardrails
    ↓
Safe Response
    ↓
User Interface

## ⚙️ Installation

1. Clone the repository

git clone https://github.com/GaddeRamesh5236/LLM--GAUARDRAILS-WORKSHOP.git

2. Navigate to the project

cd LLM--GAUARDRAILS-WORKSHOP

3. Create a virtual environment

python -m venv myvenv

4. Activate the virtual environment

.\myvenv\Scripts\Activate.ps1

5. Install dependencies

pip install -r requirements.txt

## 🔑 Environment Variables

Create a .env file in the project root:
GEMINI_API_KEY=your_gemini_api_key_here
GEMINI_MODEL=gemini-3.5-flash

## ▶️ Run the Application

Start the application with:
python app.py

## 📌 Future Improvements
Add more advanced safety checks
Add prompt injection detection
Add toxicity detection
Add PII detection
Add response quality evaluation
Add logging and monitoring
Deploy the application to the cloud
