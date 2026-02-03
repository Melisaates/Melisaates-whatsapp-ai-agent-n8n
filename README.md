# Melisaates-whatsapp-ai-agent-n8n
Multimodal AI agent workflow using n8n and OpenAI

# whatsapp-ai-agent-n8n
Multimodal AI agent workflow using n8n and OpenAI


# 🤖 WhatsApp AI Assistant Workflow (n8n + OpenAI)

An intelligent WhatsApp AI assistant built with **n8n** and **OpenAI** that supports text, voice messages, and images, and responds with text or audio while maintaining conversation memory.

---

## 📌 Repository Description

WhatsApp AI assistant workflow using n8n and OpenAI with multimodal support (text, audio, image) and conversation memory.

---

## 📝 Project Overview

This project demonstrates how to build an AI-powered WhatsApp assistant using n8n and OpenAI.  
It can receive user messages from WhatsApp, detect their type (text, audio, image), process them with OpenAI models, and automatically send intelligent replies.

The workflow is exported without credentials and sensitive data, making it safe to share and reuse.

---

## ✨ Features

- WhatsApp message trigger  
- Automatic detection of message type (Text / Audio / Image)  
- Audio transcription (speech-to-text)  
- Image analysis and description  
- AI-powered conversation agent (LangChain)  
- Conversation memory per user  
- Text-to-speech audio replies  
- Secure and reusable workflow  
- Credential-free export  

---

## 🏗 Architecture Overview

### Workflow Steps

1. WhatsApp Trigger receives incoming messages  
2. Switch node determines message type (Text / Audio / Image)  
3. Media files are downloaded if needed  
4. OpenAI processes the content  
5. AI Agent generates a response  
6. Response is sent back to the user via WhatsApp  

---

## 📊 Architecture Diagram

```text
User (WhatsApp)
      |
      v
WhatsApp Trigger (n8n)
      |
      v
Switch (Text / Audio / Image)
      |
      v
Media Download
      |
      v
OpenAI Processing
(Transcription / Image Analysis / Chat)
      |
      v
AI Agent + Memory
      |
      v
WhatsApp Response (Text or Audio)
```
⚙️ Requirements

n8n (self-hosted or cloud)

WhatsApp Business API credentials

OpenAI API key

HTTP Header Auth credentials

🚀 Installation

Clone the repository:

git clone https://github.com/your-username/your-repo-name.git


Open n8n Dashboard

Import the workflow JSON file

Configure credentials

Activate the workflow

📥 How to Import Workflow in n8n

Go to n8n Dashboard

Click Import Workflow

Upload workflow.json

Configure all required credentials

Activate the workflow

🧠 AI Behavior

The AI assistant:

Responds in a friendly and natural tone

Uses conversation memory to keep context

Can transcribe voice messages

Can analyze and describe images

Supports both text and audio responses

Automatically handles different message types

🔐 Security

This repository does NOT contain:

API keys

Credential IDs

Phone numbers

Webhook IDs

Instance IDs

All sensitive data must be configured locally in your own n8n instance.

Never commit your credentials to GitHub.

📁 Files
.
├── workflow.json
└── README.md

🛠 Customization

You can customize:

System prompt in the AI Agent node

OpenAI model (GPT-4.1-mini, GPT-4o, etc.)

Response format (text or audio)

Memory window size

Language and personality of the assistant

🧪 Testing

To test the workflow:

Send a text message to the connected WhatsApp number

Send a voice message to test transcription

Send an image to test image analysis

Verify that the AI replies correctly

🤝 Contributing

Contributions are welcome.

Steps:

Fork the repository

Create a new branch

Commit your changes

Open a Pull Request

Please ensure no credentials or sensitive data are included.

🔒 Security Policy

If you discover a security issue, please do not publish it publicly.
Contact the repository owner directly.

📄 License

This project is provided for educational and demonstration purposes only.

🙋 Author

Developed by Melisa Ateş

⭐ Acknowledgements

n8n

OpenAI

WhatsApp Business API

LangChain
