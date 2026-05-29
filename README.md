# Secure File Sharing System

## Overview
A web-based platform for sharing files with end-to-end encryption, access controls, and audit logging.

## Tools & Technologies
- **Python** – Backend (Flask/FastAPI)
- **Encryption** – AES-256 for file encryption, RSA for key exchange
- **MySQL** – User management, file metadata, access logs
- **Node.js** – Frontend server
- **Pandas** – Audit log analysis and reporting

## Project Structure
```
secure_file_sharing_system/
├── backend/
│   ├── app.py
│   ├── encryption/
│   │   ├── aes_handler.py
│   │   └── rsa_handler.py
│   ├── routes/
│   └── models/
├── frontend/
│   └── public/
├── database/
│   └── schema.sql
├── audit/
│   └── log_analyzer.py
└── README.md
```

## Features
- File upload with AES-256 encryption at rest
- RSA key exchange for secure sharing between users
- Role-based access control (owner, viewer, editor)
- Download tokens with expiry
- Full audit trail stored in MySQL

## Setup
```bash
pip install -r requirements.txt
python backend/app.py
```
