# AI-Powered Healthcare Chatbot using GPT-2

This project demonstrates a healthcare-focused AI chatbot that answers medical questions using a GPT-2 model fine-tuned on the MedQuad dataset. It supports features like appointment booking, medication reminders, and SMS notifications via Twilio.

## 🔍 Features

- GPT-2 chatbot fine-tuned on medical Q&A (MedQuad)
- Flask REST API for chatbot and scheduling
- SQLite database for storing appointments and reminders
- APScheduler for scheduling medication reminders
- Twilio integration for SMS alerts

## 🧠 Model

- Model: GPT-2 (via Hugging Face)
- Dataset: MedQuad
- Fine-tuning: PyTorch & Hugging Face Transformers

## 📁 File Structure

ChatbotGPT.ipynb            → Main implementation notebook
healthcare.db               → SQLite database (appointments & reminders)
ChatbotGPT_report.pdf       → Full technical report
README.md                   → Project documentation
.gitignore                  → Files to be ignored by Git

## 🛠️ API Endpoints

- `/general_info` → Responds to medication-related queries  
- `/book_appointment` → Book a doctor’s appointment  
- `/set_reminder` → Schedule a medication reminder  

## 🔔 Reminder Functionality

Twilio SMS reminders notify users based on the schedule set through the API.

## 📦 Tech Stack

- GPT-2 (HuggingFace)  
- Flask  
- SQLite  
- APScheduler  
- Twilio  

## 📚 Report

See [ChatbotGPT_report.pdf](ChatbotGPT_report.pdf) for a full explanation.

---

## ⚙️ Setup Instructions

```bash
pip install flask transformers twilio apscheduler

Start the Flask server (refer to ChatbotGPT.ipynb for the implementation).

⸻

🧪 Testing

Use Postman or cURL to test endpoints:
	•	/general_info
	•	/book_appointment
	•	/set_reminder

⸻

👨‍⚕️ Future Enhancements
	•	Multilingual query support
	•	Integration with voice assistants
	•	Customizable recurring reminders
	•	Deployment to cloud (Docker + FastAPI)

⸻

🔗 References
	•	GPT-2 on HuggingFace
	•	MedQuad Dataset
	•	Flask Docs
	•	Twilio SMS API
