<div align="center">
  <br />
    <img src="public/icons/logo.svg" alt="Project Banner" width="120">
  <br />

  <div>
    <img src="https://img.shields.io/badge/-Next_JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
    <img src="https://img.shields.io/badge/-TypeScript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
    <img src="https://img.shields.io/badge/-Appwrite-black?style=for-the-badge&logoColor=white&logo=appwrite&color=FD366E" alt="appwrite" />
  </div>

  <h3 align="center">Banking Web App</h3>
  <p align="center">A modern fintech web application for connecting bank accounts, tracking transactions, and transferring funds.</p>
</div>

## Table of Contents

1. Introduction
2. Tech Stack
3. Features
4. Quick Start
5. Environment Variables
6. Scripts
7. License

## Introduction

This application lets users connect multiple bank accounts, view real-time balances and transactions, and transfer funds to other users. It uses a modern Next.js (App Router) stack with secure server-side flows.

## Tech Stack

- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS
- Appwrite (auth + database)
- Plaid (bank account linking)
- Dwolla (funds transfer)
- React Hook Form + Zod
- Chart.js

## Features

- Authentication with validation and authorization
- Link multiple bank accounts (Plaid)
- Real-time balance and transaction views
- Transaction history with filters and pagination
- Funds transfer via Dwolla
- Responsive UI and reusable components

## Quick Start

Prerequisites:
- Node.js 18+
- npm

Install dependencies:

```bash
npm install
```

Create a `.env` file and configure the variables listed below. You can copy from `.env.example` and fill in your values.

Run the dev server:

```bash
npm run dev
```

Build and start:

```bash
npm run build && npm start
```

## Environment Variables

See `.env.example` for the full list. Key variables:

- NEXT_PUBLIC_SITE_URL
- NEXT_PUBLIC_APPWRITE_ENDPOINT, NEXT_PUBLIC_APPWRITE_PROJECT, NEXT_APPWRITE_KEY
- APPWRITE_DATABASE_ID, APPWRITE_USER_COLLECTION_ID, APPWRITE_ITEM_COLLECTION_ID, APPWRITE_BANK_COLLECTION_ID, APPWRITE_TRANSACTION_COLLECTION_ID
- PLAID_CLIENT_ID, PLAID_SECRET, PLAID_ENV, PLAID_PRODUCTS, PLAID_COUNTRY_CODES
- DWOLLA_KEY, DWOLLA_SECRET, DWOLLA_BASE_URL, DWOLLA_ENV
- SENTRY_DSN, NEXT_PUBLIC_SENTRY_DSN (optional)

## Scripts

- `npm run dev` — Start dev server
- `npm run build` — Create production build
- `npm start` — Start production server
- `npm run lint` — Lint code

## License

This project is licensed under the MIT License. See `LICENSE` for details.

