# Docker Fullstack App (React + Flask)

A minimal fullstack boilerplate using **React** for the frontend and **Flask** for the backend, orchestrated via **Docker Compose**.

## Tech Stack

- **Frontend**: React
- **Backend**: Flask (Python)
- **Containerization**: Docker & Docker Compose

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yyuni915/docker-fullstack-app.git
cd docker-fullstack-app
```

### 2. Run the Application
Make sure you have Docker and Docker Compose installed. Then, run:
```bash
docker compose up --build
```

This will:
Build the React frontend (localhost:3000)
Build the Flask backend (localhost:5000)

###  Project Structure
```bash
docker-fullstack-app/
│
├── backend/               # Flask app
│   ├── app.py
│   ├── Dockerfile
│   ├── requirements.txt
│   └── .env
│
├── frontend/              # React app
│   ├── Dockerfile
│   ├── node_modules/
│   └── ...
│
├── docker-compose.yml     # Compose config for both services
└── README.md
```

### API Communication

Frontend makes API calls to: http://localhost:5000/

Backend response example:
```json
{ "message": "Hello from Flask!" }
```

### Author
Yuni Yoon
