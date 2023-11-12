# Full Stack E-Commerce + Dashboard & CMS: Next.js 13 App Router, React, Tailwind, Prisma, MySQL, 2023

This repository features a Next.js 13 App Router, React, Tailwind, Prisma, and MySQL stack, creating an inclusive Full Stack E-Commerce + Dashboard & CMS where users can effortlessly manage multiple stores, categories, products, and dynamic content like billboards, all with Clerk Authentication, Stripe integration, and insightful revenue analytics. The robust backend relies on MySQL, Prisma, and PlanetScale for scalability.

### Prerequisites
**Node version 14.x**
### Install packages
```shell
npm i
```
### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```
### Connect to PlanetScale and Push Prisma
```shell
npx prisma generate
npx prisma db push
```
### Start the app

```shell
npm run dev
```

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
