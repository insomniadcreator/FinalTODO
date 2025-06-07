# Full-Stack Web Application

This project is a full-stack web application built with:

## Frontend
- React
- TypeScript
- React Router
- Axios

## Backend
- Python (FastAPI)
- PostgreSQL
- SQLAlchemy ORM
- Celery + RabbitMQ for task queues

## Getting Started

### Prerequisites
- Node.js and npm
- Python 3.8+
- PostgreSQL
- RabbitMQ

### Installation

#### Backend
1. Navigate to the backend directory:
```
cd backend
```

2. Create a virtual environment:
```
python -m venv venv
```

3. Activate the virtual environment:
- Windows:
```
venv\Scripts\activate
```
- macOS/Linux:
```
source venv/bin/activate
```

4. Install dependencies:
```
pip install -r requirements.txt
```

5. Set up the database:
```
alembic upgrade head
```

6. Start the backend server:
```
uvicorn app.main:app --reload
```

#### Frontend
1. Navigate to the frontend directory:
```
cd frontend
```

2. Install dependencies:
```
npm install
```

3. Start the development server:
```
npm start
```

## Project Structure
```
.
├── backend/                # FastAPI backend
│   ├── alembic/            # Database migrations
│   ├── app/                # Application code
│   │   ├── api/            # API endpoints
│   │   ├── core/           # Core components (config, security, etc.)
│   │   ├── db/             # Database models and sessions
│   │   ├── schemas/        # Pydantic schemas
│   │   ├── services/       # Business logic
│   │   ├── tasks/          # Celery tasks
│   │   └── main.py         # Application entry point
│   ├── tests/              # Unit and integration tests
│   └── requirements.txt    # Python dependencies
├── frontend/               # React frontend
│   ├── public/             # Static files
│   ├── src/                # Source code
│   │   ├── components/     # React components
│   │   ├── pages/          # Page components
│   │   ├── services/       # API services
│   │   ├── styles/         # CSS/SCSS files
│   │   ├── types/          # TypeScript type definitions
│   │   ├── utils/          # Utility functions
│   │   ├── App.tsx         # Main App component
│   │   └── index.tsx       # Entry point
│   ├── package.json        # NPM dependencies
│   └── tsconfig.json       # TypeScript config
└── docker-compose.yml      # Docker configuration
```
