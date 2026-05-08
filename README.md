# Express API Quick Starter

A RESTful API starter template built with Express.js featuring JWT authentication, MongoDB integration, and Passport.js for secure user management.

## Tech Stack

| Technology | Purpose |
|------------|---------|
| Node.js | Runtime environment |
| Express.js | Web framework |
| MongoDB | Database |
| Mongoose | ODM for MongoDB |
| Passport.js | Authentication middleware |
| JWT | Token-based authentication |
| bcrypt-nodejs | Password hashing |

## Features

- JWT-based authentication
- User registration and login
- Password encryption with bcrypt
- MongoDB database integration
- Modular route structure
- Database seeding
- Environment-based configuration
- Request logging with Morgan

## Prerequisites

- Node.js (v8.x or higher)
- MongoDB (local or remote instance)
- npm or yarn

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/nikolaykolibarov/express-api-quick-starter.git
   cd express-api-quick-starter
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure the database connection in `config/config.js`

## How to Run

Start the development server:
```bash
npm start
```

The API will be available at `http://localhost:3000` (or the port configured in your config).

## Project Structure

```
express-api-quick-starter/
├── config/
│   ├── config.js        # Environment configuration
│   ├── database.js      # MongoDB connection
│   ├── express.js       # Express middleware setup
│   ├── passport.js      # Passport JWT strategy
│   ├── routes.js        # Route configuration
│   └── seeder.js        # Database seeder
├── middlewares/
│   └── auth.js          # Authentication middleware
├── users/
│   ├── User.js          # User model
│   ├── users-controller.js  # User controller
│   ├── users-routes.js  # User routes
│   └── users-seeder.js  # User seeder
├── server.js            # Application entry point
└── package.json
```

> **Note:** This project was created for educational/course purposes and serves as a learning resource for building RESTful APIs with Express.js and JWT authentication.
