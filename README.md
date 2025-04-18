# Personal Finance Tracker

A full-stack application for tracking personal finances, built with FastAPI (backend) and React (frontend).

## Project Structure

```
personal-finance-tracker/
├── backend/                 # FastAPI backend service
│   ├── user_service/       # User authentication service
│   │   ├── app/           # Application code
│   │   ├── tests/         # Test files
│   │   ├── requirements.txt
│   │   └── Dockerfile
├── frontend/               # React frontend
│   ├── src/               # Source code
│   ├── public/            # Static files
│   ├── package.json
│   └── Dockerfile
├── docker-compose.yml     # Docker compose configuration
└── .env.example          # Environment variables template
```

## Prerequisites

- Docker and Docker Compose
- Python 3.8+
- Node.js 14+
- npm or yarn

## Setup

1. Clone the repository
2. Copy `.env.example` to `.env` and update the variables
3. Run the application using Docker Compose:
   ```bash
   docker-compose up --build
   ```

## Development

### Backend

- FastAPI
- SQLAlchemy
- PostgreSQL
- JWT Authentication

### Frontend

- React
- Material-UI
- Axios
- React Router

## API Documentation

Once the application is running, you can access the API documentation at:

- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## License

MIT
