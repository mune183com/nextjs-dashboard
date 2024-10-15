## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## Project Setup

### Environment Variables

To run this project, you will need to add the following environment variables to your `.env.local` file:

```
# Copy from .env.local on the Vercel dashboard
# https://nextjs.org/learn/dashboard-app/setting-up-your-database#create-a-postgres-database
POSTGRES_URL=
POSTGRES_PRISMA_URL=
POSTGRES_URL_NON_POOLING=
POSTGRES_USER=
POSTGRES_HOST=
POSTGRES_PASSWORD=
POSTGRES_DATABASE=

# `openssl rand -base64 32`
AUTH_SECRET=
AUTH_URL=http://localhost:3000/api/auth
```

### Database Setup

1. Create a PostgreSQL database.
2. Update the environment variables in your `.env.local` file with your database credentials.
3. Run the following command to create the necessary tables:

```bash
npm run seed
```

### Running the Application

To run the application, use the following commands:

```bash
# Install dependencies
npm install

# Run the application in development mode
npm run dev

# Build the application for production
npm run build

# Start the application in production mode
npm start
```

## Seeding the Database

To seed the database with initial data, use the provided `scripts/seed.js` script. Run the following command:

```bash
npm run seed
```

## Running Linting and Formatting Checks

To run linting and formatting checks, use the following commands:

```bash
# Run linting checks
npm run lint

# Run formatting checks
npm run prettier:check

# Automatically fix formatting issues
npm run prettier
```
