
# Jobly (backend)

Jobly is a job listing and application management system built with Node.js, Express, PostgreSQL, and JWT for user authentication. This application allows users to browse jobs, apply for positions, and manage company listings.

## Installation

To get started, clone the repository and install the necessary dependencies.

```bash
git clone git@github.com:NihalChehade/jobly-backend.git
cd jobly-backend
npm install
```

## Setup
Create a `.env` file in the root directory of your project. Add the following environment variables:

    ```
    SECRET_KEY= your-secret-key
    DATABASE_URL=your-production-database-url
    PORT=3001
    ```

### Database Setup

To set up the database, you will need PostgreSQL installed.

1. Create the databases:

    ```bash
    createdb jobly
    createdb jobly_test
    ```

2. Use the provided SQL files to create tables and seed data:

    ```bash
    psql jobly < jobly-schema.sql
    psql jobly < jobly-seed.sql
    ```

3. Update your `.env` file to include the test database URI for testing:

    ```
    DATABASE_URL_TEST=postgresql://username:password@localhost:5432/jobly_test
    ```

4. If necessary, modify `config.js` to point to your local or production database.

## Technologies

- **Node.js**: JavaScript runtime.
- **Express.js**: Fast, unopinionated, minimalist web framework for Node.js.
- **PostgreSQL**: Powerful, open-source object-relational database.
- **JWT (jsonwebtoken)**: Secure user authentication.
- **bcrypt**: Secure password hashing.
- **Jest & Supertest**: Testing frameworks.


## Running the Application

You can start the application in development mode using `nodemon` or start it normally using `node`.

```bash
# For development mode
npm run dev

# For production mode
npm run start
```

By default, the app runs on `http://localhost:3001`. You can change the port in the `.env` file.

## Running Tests

The application uses `Jest` and `supertest` for testing. To run the tests, execute the following command:

```bash
npm run test
<<<<<<< HEAD
```
=======
```




>>>>>>> b5074a7295588ac12ae6bdf9d80ca9613e2f39b5
