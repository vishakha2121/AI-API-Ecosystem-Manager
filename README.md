# 🤖 AI Autonomous API Ecosystem Manager

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.95+-green.svg)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18-61DAFB.svg)](https://reactjs.org/)
[![LangGraph](https://img.shields.io/badge/LangGraph-AI-orange.svg)](https://langchain.ai/)
[![Gemini](https://img.shields.io/badge/Gemini-AI-purple.svg)](https://deepmind.google/technologies/gemini/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue.svg)](https://www.postgresql.org/)
[![Redis](https://img.shields.io/badge/Redis-7-red.svg)](https://redis.io/)
[![Docker](https://img.shields.io/badge/Docker-24-blue.svg)](https://www.docker.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 📋 Overview

An **AI-powered autonomous API ecosystem manager** that uses collaborative AI agents to **monitor**, **secure**, **test**, **optimize**, and **document** thousands of APIs. Built with **LangGraph** orchestration and **Google Gemini AI**, this platform simulates a real-world API management solution for learning and practice.

> **Note:** This is a practice project designed for learning and portfolio demonstration. Not intended for production deployment.

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| 🤖 **AI Agents** | 6 specialized agents working collaboratively using LangGraph |
| 📊 **Real-time Monitoring** | Continuous API health checks with alerts and analytics |
| 🔒 **Security Scanning** | Automated vulnerability detection and risk assessment |
| 🧪 **Automated Testing** | End-to-end API testing with comprehensive reporting |
| ⚡ **Optimization** | AI-powered performance recommendations and improvements |
| 📝 **Documentation** | Auto-generated, versioned API documentation |
| 🎯 **API Gateway** | Centralized routing, rate limiting, and caching |
| 🎨 **Modern UI** | Beautiful React dashboard with real-time updates |

---

## 🛠️ Tech Stack

### Backend
- **Python 3.10+** - Core language
- **FastAPI** - Web framework
- **LangGraph** - AI agent orchestration
- **Gemini AI** - Language model for intelligent decisions
- **PostgreSQL** - Primary database
- **Redis** - Cache & message broker
- **Celery** - Async task queue
- **SQLAlchemy** - ORM
- **JWT** - Authentication

### Frontend
- **React 18** - UI framework
- **Vite** - Build tool
- **TailwindCSS** - Styling
- **Chart.js** - Charts & visualizations
- **React Router v6** - Routing
- **Axios** - HTTP client
- **Socket.io** - WebSocket for real-time updates
- **Framer Motion** - Animations

### DevOps
- **Docker** - Containerization
- **Nginx** - Web server
- **Git** - Version control

---

## 🏗️ Architecture

### AI Agents (LangGraph)

### Workflow

1. User sends request to API endpoint
2. Orchestrator agent analyzes request
3. Routes to appropriate specialized agent
4. Agent processes request using Gemini AI
5. Returns results with intelligent insights
6. Updates dashboard in real-time

---

## 📁 Project Structure

---

## 🚀 Quick Start

### Prerequisites

- Python 3.10+
- Node.js 18+
- PostgreSQL 15+
- Redis 7+
- Docker (optional)

### 1️⃣ Clone Repository

```bash
git clone https://github.com/vishakha2121/AI-API-Ecosystem-Manager.git
cd AI-API-Ecosystem-Manager

cd backend

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env
# Edit .env with your configurations

# Setup database
createdb api_manager
alembic upgrade head

# Seed initial data
python scripts/seed_data.py

# Run backend server
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

cd frontend

# Install dependencies
npm install

# Create .env file
cp .env.example .env
# Edit .env with your configurations

# Run frontend server
npm run dev