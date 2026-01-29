MediMate Chain – Blockchain-Enabled AI Healthcare Assistant
🎯 Overview

MediMate Chain is a full-stack, blockchain-enabled, AI-powered healthcare application that automates pre-consultation clinical history collection while ensuring data integrity, patient consent, and transparency.

It combines AI + Web3 + modern web technologies to give patients ownership of their medical data and help doctors prepare better before consultations.

Built with FastAPI, React, MongoDB, Smart Contracts, and OpenAI models.

✨ Features
For Patients

--- 🔐 Secure authentication using wallet-based login with role mapping
--- 👨‍⚕️ Doctor selection and appointment booking
--- 💬 AI chatbot for interactive pre-consultation medical history collection
--- 🎤 Voice input and output using OpenAI Whisper & TTS
--- 📸 Image upload with AI-based symptom analysis
--- 🔏 Consent management to grant or revoke doctor access
--- 📜 Blockchain verification of medical summaries

For Doctors

--- 📊 Doctor dashboard with appointment overview
--- 📄 AI-generated patient summaries before consultation
--- 🔍 Patient search and filtering
--- 🔗 Blockchain-verified summary authenticity
--- 💾 Export summaries as JSON with on-chain hash
--- 🧾 Immutable audit trail of patient consent

🚀 Quick Start

Demo Credentials:

Patient: patient@demo.com / 12345
Doctor: doctor@demo.com / admin123

💡 How It Works

Patient books an appointment with a doctor

AI Chatbot conducts a structured pre-consultation interview

Patient shares symptoms via text, voice, or images

AI generates a structured clinical summary

Summary is stored off-chain in MongoDB

Hash of the summary is stored on the blockchain

Doctor reviews and verifies the summary before consultation

🏗️ Tech Stack

--- Backend: FastAPI (Python)
--- Frontend: React + shadcn/ui
--- Database: MongoDB (off-chain storage)
--- Blockchain: Solidity smart contracts (consent & summary hashes)
--- AI: OpenAI GPT-4o, Whisper, TTS, Vision
--- Authentication: Wallet auth + JWT mapping

📁 Project Structure
MediMate-Chain/
├── backend/
│   ├── server.py          # FastAPI application
│   ├── blockchain/        # Web3 & smart contract interaction
│   ├── ai/                # Chatbot & summarization logic
│   ├── .env
│   └── requirements.txt
├── smart-contracts/
│   ├── ConsentManager.sol # Consent & summary hash contract
│   └── deploy.js
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── context/
│   │   └── web3/
│   └── package.json
└── README.md

🗄️ Database Collections

--- users – Patient and doctor accounts
--- appointments – Scheduled consultations
--- chat_messages – AI conversation history
--- summaries – AI-generated clinical summaries

On-Chain Data:
--- summaryHash
--- patientAddress
--- doctorAddress
--- consentStatus
--- timestamp

🔧 API Endpoints
Auth

--- POST /api/auth/wallet-login – Wallet authentication
--- POST /api/auth/role-assign – Assign patient or doctor role

Patient

--- GET /api/patient/doctors – List doctors
--- POST /api/patient/book – Book appointment
--- POST /api/patient/consent – Grant or revoke consent

Chat

--- POST /api/chat/message – Send message
--- POST /api/chat/voice – Voice input
--- POST /api/chat/upload – Upload image
--- POST /api/chat/end – Generate summary

Doctor

--- GET /api/doctor/appointments – List appointments
--- GET /api/doctor/summary/:id – View summary
--- GET /api/doctor/verify – Verify on-chain hash

🎨 Features Showcase

--- Modern medical-themed UI
--- Voice-enabled AI chat interface
--- Image analysis with AI vision models
--- Real-time AI responses
--- Blockchain-verified medical summaries
--- Role-based dashboards
--- Responsive and mobile-friendly design

Built with ❤️ for secure, transparent, and intelligent healthcare.
