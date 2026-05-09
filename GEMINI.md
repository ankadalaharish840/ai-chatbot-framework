# Chatbot Application - Gemini AI Context

> **Project Context for AI Assistants**  
> This document provides essential context about the Chatbot application for AI-assisted development.

## Project Overview

**Name:** Chatbot  
**Framework:** Flask (Python) + React Frontend  
**Infrastructure:** Docker, Kubernetes (Helm)  
**Type:** Full-stack conversational AI application

## Project Purpose

A conversational AI chatbot application featuring:
- Flask backend with REST API
- React frontend for chat interface
- Docker containerization
- Kubernetes deployment via Helm charts
- LLM integration support

## Key Technologies

| Technology | Purpose |
|------------|---------|
| Python/Flask | Backend API |
| React | Frontend UI |
| Docker | Containerization |
| Helm | Kubernetes deployment |
| PostgreSQL | Database (via migrations) |

## Directory Structure

```
chatbot/
├── app/               # Flask application
├── frontend/          # React frontend
├── helm/             # Kubernetes Helm charts
├── migrations/       # Database migrations
├── scripts/          # Utility scripts
├── tests/            # Test suite
├── examples/         # Usage examples
├── docs/             # Documentation
├── docker-compose.yml       # Docker orchestration
├── docker-compose.dev.yml   # Development config
├── docker-compose.llm.yml   # LLM-specific config
├── Dockerfile        # Container definition
├── requirements.txt  # Python dependencies
├── config.py        # Flask configuration
├── manage.py        # Django-style management
└── run.py           # Application entry point
```

## Build Commands

```bash
# Development with Docker Compose
docker-compose -f docker-compose.dev.yml up

# Production deployment
docker-compose up -d

# LLM-enabled deployment
docker-compose -f docker-compose.llm.yml up

# Run locally without Docker
pip install -r requirements.txt
python run.py
```

## Key Files

- [config.py](config.py) - Flask configuration
- [requirements.txt](requirements.txt) - Python dependencies
- [CONTRIBUTING.md](CONTRIBUTING.md) - Contribution guidelines
- [docs/](docs/) - Detailed documentation
