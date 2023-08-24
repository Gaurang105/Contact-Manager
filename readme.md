# Contact Manager

Contact Manager is a backend application developed using Node.js, Express, MongoDB, and JWT. The application provides functionalities to manage contacts and users with CRUD (Create, Read, Update, Delete) operations.

## Table of Contents

- [Getting Started](#getting-started)
- [Endpoints](#endpoints)
- [Middleware](#middleware)
- [Controllers](#controllers)
- [Database Connection](#database-connection)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

### Prerequisites

- Node.js
- MongoDB

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/Contact-Manager.git
   ```

2. **Navigate to Project Directory**
   ```bash
   cd Contact-Manager
   ```

3. **Install Dependencies**
    ```bash
    npm install
    ```

4. **Create .env File**
   Add your environment variables such as `PORT`, `ACCESS_TOKEN_SECRET`, and `CONNECTION_STRING`.

5. **Run the Server**
    ```bash
    npm start
    ```

## Endpoints

### Users

- Register: `POST /api/users/register`
- Login: `POST /api/users/login`
- Current User: `GET /api/users/current`

### Contacts

- Get all: `GET /api/contacts`
- Create: `POST /api/contacts`
- Get by ID: `GET /api/contacts/:id`
- Update by ID: `PUT /api/contacts/:id`
- Delete by ID: `DELETE /api/contacts/:id`

## Middleware

### ErrorHandler

Handles various types of errors, including validation, unauthorized access, and server errors.

### ValidateTokenHandler

Verifies and validates the JWT token for protected routes.

## Controllers

### Contact Controller

Handles operations related to contacts such as fetching all contacts, creating, updating, and deleting contacts.

### User Controller

Manages user-related operations such as registration, login, and fetching the current user information.

## Database Connection

`dbConnection.js` manages the connection to the MongoDB database using Mongoose.

## Contributing

Feel free to fork, open pull requests, or submit issues.

## License

MIT License
