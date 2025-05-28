# cst8919-Lab 1: Auth0 Python Web App Integration

This project demonstrates how to implement secure login and logout functionality in a Python Flask application using Auth0. It includes a protected route accessible only by authenticated users.

## Features

- Secure login/logout using [Auth0](https://auth0.com/)
- Session management using Flask
- Protected route (`/protected`)
- Auth0 user information displayed on dashboard
- Environment variables used for secrets

---
## Getting Started

### Prerequisites

- Python 3.10+
- GitHub account
- Auth0 account
- VSCode with Remote - WSL extension (if using WSL)

---
## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/alkh0115/cst8919-lab1-auth0
cd cst8919-lab1-auth0
```
### 2. Create a Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```
### 3. Install Dependencies

```bash
pip install -r requirements.txt
```
### 4. Configure Auth0 Environment Variables

```bash
AUTH0_CLIENT_ID=your-client-id
AUTH0_CLIENT_SECRET=your-client-secret
AUTH0_DOMAIN=your-tenant-region.auth0.com
APP_SECRET_KEY=generate-a-random-secret-key
```
You can generate a secure APP_SECRET_KEY using:

```bash
openssl rand -hex 32
```
---
## Run the App

```bash
source venv/bin/activate
python server.py
```
Then open your browser and navigate to:

```bash
http://localhost:3000
```
You can:

- Access the public homepage
- Click “Login” to authenticate via Auth0
- View /dashboard and /protected routes if logged in
- Click “Logout” to end session

### Protected Route
The /protected route is only accessible to authenticated users. If a user is not logged in, they will be redirected to the login screen.

---
## Demo Video:
Please visit the link: 






