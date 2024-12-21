# JWTNestAPI

## Project Description
A NestJS-based API to manage CRUD operations with PostgreSQL using TypeORM, including authentication with JWT. This project is a comprehensive example of implementing robust backend services with proper authentication and error handling.

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Project Setup](#project-setup)
- [Environment Variables](#environment-variables)
- [Compile and Run](#compile-and-run)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Deployment](#deployment)
- [Changing End of Line Sequence](#changing-end-of-line-sequence)
- [Resources](#resources)
- [Support](#support)
- [Stay in Touch](#stay-in-touch)
- [License](#license)

## Features
- NestJS framework for scalable server-side applications.
- PostgreSQL database with TypeORM for data interaction.
- JWT-based authentication and authorization.
- CRUD operations for user management.
- Comprehensive unit tests with Jest.
- Detailed error handling and input validation.

## Project Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/TtarunNDeveloper/JWTNestAPI.git
2. Navigate to the project directory:
  cd JWTNestAPI
3. Install dependencies:
  npm install

## Environment Variables
Create a .env file in the root of your project and add the following variables:
  JWT_SECRET=yourSecretKeyHere
  DATABASE_HOST=localhost
  DATABASE_PORT=5432
  DATABASE_USERNAME=yourUsername
  DATABASE_PASSWORD=yourPassword
  DATABASE_NAME=yourDatabaseName

## Compile and Run
  # development
    npm run start
  # watch mode
    npm run start:dev
  # production mode
    npm run start:prod
  
# Access the API at: 
  http://localhost:3000

# API Endpoints
  Register a New User:
    Method: POST
    URL: /users
    Body: json
    {
      "name": "John Doe",
      "email": "john.doe@example.com",
      "password": "securePassword123"
    }
  
  Login:
    Method: POST
    URL: /auth/login
    Body: json
    {
      "email": "john.doe@example.com",
      "password": "securePassword123"
    }
  
  Access Protected Route(Profile):
    Method: POST
    URL: /auth/profile
    Headers: json
    {
      "Authorization": "Bearer your_jwt_token_here"
    }

# Testing
  1.Run Tests:
    # unit tests
    npm run test
    # end-to-end tests
    npm run test:e2e
    # test coverage
    npm run test:cov
 
# Deployment
  For deployment, follow https://docs.nestjs.com/deployment

# Changing End of Line Sequence
  If you encounter issues related to the End of Line Sequence (EOL), you can change it from CRLF to LF:

  1.In VSCode, open Command Palette (Ctrl+Shift+P).

  2.Type Change End of Line Sequence and select it.

  3.Choose LF to change the EOL sequence.

