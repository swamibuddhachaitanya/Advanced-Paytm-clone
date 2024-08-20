
# Advanced Paytm Clone

An advanced version of an online wallet system similar to Paytm, featuring user login, email/phone authentication, bank on/off ramp integration, and phone/name-based transfers. Built with a modern tech stack including Next.js, Express, Turborepo, Postgres, Prisma ORM, and Tailwind.

## Features

- **User Authentication:** Secure login with email or phone number.
- **Bank Integration:** On-ramp and off-ramp support for bank transfers.
- **Seamless Transfers:** Transfer money via phone number or name.

## Tech Stack

- **Frontend/Backend:** Next.js
- **Auxiliary Backends:** Express.js
- **Monorepo Management:** Turborepo
- **Database:** Postgres
- **ORM:** Prisma
- **Styling:** Tailwind CSS

## Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

- **Node.js** and **npm** installed.
- **Postgres** running locally or on a cloud service like [neon.tech](https://neon.tech).

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/swamibuddhachaitanya/Advanced-Paytm-clone
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up Postgres:**

   Run Postgres locally using Docker:

   ```bash
   docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
   ```

4. **Environment Variables:**

   - Copy all `.env.example` files to `.env`:
   - Update `.env` files with the correct database URL and other environment variables.

5. **Database Setup:**

   Navigate to the `packages/db` directory:

   ```bash
   cd packages/db
   ```

   - Run migrations:

     ```bash
     npx prisma migrate dev
     ```

   - Seed the database:

     ```bash
     npx prisma db seed
     ```

6. **Running the Application:**

   Navigate to the `apps/user-app` directory:

   ```bash
   cd apps/user-app
   ```

   - Start the development server:

     ```bash
     npm run dev
     ```

7. **Login:**

   - Try logging in using:
     - **Phone:** `1111111111`
     - **Password:** `alice` (This is part of the seeded data in `seed.ts`)

