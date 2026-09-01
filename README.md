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



### 🔄 Application Flow


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
