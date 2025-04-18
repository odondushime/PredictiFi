# Personal Finance Tracker

Hey there! 👋 This is a personal finance tracking app I built to help manage my money better. It's a full-stack application that lets you track expenses, set budgets, and get insights into your spending habits.

## What's Inside

The app is split into two main parts:

- **Backend**: Built with FastAPI, it handles all the data and authentication
- **Frontend**: A React app that makes everything look pretty and easy to use

Here's how everything's organized:

```
personal-finance-tracker/
├── backend/                 # The brains of the operation
│   ├── user_service/       # Handles all the user stuff
│   │   ├── app/           # Where the magic happens
│   │   ├── tests/         # Making sure everything works
│   │   ├── requirements.txt
│   │   └── Dockerfile
├── frontend/               # The pretty face
│   ├── src/               # All the React components
│   ├── public/            # Static files
│   ├── package.json
│   └── Dockerfile
├── docker-compose.yml     # Ties everything together
└── .env.example          # Template for your settings
```

## Getting Started

You'll need a few things to run this locally:

- Docker and Docker Compose
- Python 3.8 or later
- Node.js 14 or later
- npm or yarn

Here's how to get it running:

1. Clone this repo
2. Copy `.env.example` to `.env` and fill in your settings
3. Fire it up with:
   ```bash
   docker-compose up --build
   ```

## Tech Stack

### Backend

- FastAPI - Super fast Python framework
- SQLAlchemy - For talking to the database
- PostgreSQL - Where all the data lives
- JWT - For keeping things secure

### Frontend

- React - For building the UI
- Material-UI - Makes everything look nice
- Axios - For talking to the backend
- React Router - For moving around the app

## API Docs

Once everything's running, you can check out the API docs:

- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## License

This project is open source and available under the MIT License. Feel free to use it, modify it, or contribute to it!

## About Me

I'm always looking to improve this project. If you have any suggestions or find any bugs, feel free to open an issue or submit a pull request. Let's make personal finance management better together!

Github: https://github.com/odondushime
LinkeIn: www.linkedin.com/in/odon-dushime-276b9b271
