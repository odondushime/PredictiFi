# My Personal Finance Tracker

I've been working on a platform to really get a handle on my finances. It's built to live in the cloud, so I can access it anywhere, and it helps me keep tabs on my budgets and where my money is going. The cool part is it even tries to predict my future spending using some smart analysis I've built in. Everything is designed to be super secure under the hood.

## What It Does

  - Lets me set up budgets and automatically sorts my expenses.
  - Gives me a heads-up on where my spending might be heading.
  - Uses secure methods to protect my data when it talks to other services.
  - Processes my transactions quickly and reliably.

## How It's Built

  - **The Brains (Backend)**: I used Python with FastAPI to build the core logic.
  - **What You See (Frontend)**: React handles the user interface.
  - **Where It Lives (Cloud)**: It's all running on AWS using things like ECS, RDS, and Kafka.
  - **The Smart Stuff (AI)**: scikit-learn helps with the predictions.
  - **Where the Data Lives (Database)**: PostgreSQL keeps everything organized.
  - **Keeping Things Separate (Containerization)**: Docker helps manage all the different parts.

## The Big Picture

It's broken down into different services for managing users, processing transactions, and doing the analysis. They all talk to each other using Kafka, which helps it handle a lot of activity smoothly.

## Getting It Running

1.  First, you grab the code: `git clone https://github.com/yourusername/personal-finance-platform`
2.  Then, you install the necessary tools: `pip install -r requirements.txt` for the backend and `npm install` for the frontend.
3.  You'll need to set up your AWS access and create a `.env` file based on the `.env.example` file.
4.  To run it on your computer, just use: `docker-compose up`
5.  You can see it in your browser at `http://localhost:3000`

## How to Use It

  - Sign up at `/auth/register`
  - Create your budgets through `/budgets`
  - Check out the spending insights at `/insights`

## Keeping Things Safe

  - It uses OAuth 2.0 to make sure only you can access your account.
  - Sensitive information is protected with AES-256 encryption.
  - I've followed secure coding practices based on OWASP guidelines.

## Making Sure It Works

You can run the tests with `pytest tests/`. This checks both the individual parts and how they work together.

## Staying Up-to-Date

I've set up a GitHub Actions pipeline that automatically checks the code, runs tests, and deploys updates to AWS (see `.github/workflows/ci.yml`).

## What's Next

  - I'm planning to add support for different currencies.
  - I also want to integrate real-time notifications and more features down the line.

-----

This is a project by me, Odon Dushime. Feel free to connect on LinkedIn: [www.linkedin.com/in/odon-dushime-276b9b271](https://www.linkedin.com/in/odon-dushime-276b9b271).
