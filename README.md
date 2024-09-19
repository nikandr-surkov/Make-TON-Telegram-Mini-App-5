# Make TON Telegram Mini App 5: Connect to MongoDB Database With Prisma, Create New User

Welcome to the fifth guide in the **Make TON Telegram Mini App** series! This project demonstrates how to connect a Telegram Mini App to a MongoDB database using Prisma ORM, and implement user creation functionality using Next.js 14 and TypeScript.

## Project Overview

This Telegram Mini App showcases:
- Setting up a Next.js 14 project with TypeScript and Tailwind CSS
- Connecting to MongoDB using Prisma ORM
- Implementing user creation and retrieval
- Handling Telegram user data
- Managing user points system
- Basic error handling and data validation

## Prerequisites

- Node.js (version 14 or higher)
- npm (comes with Node.js)
- A Telegram account
- A Telegram Bot Token
- GitHub account
- Vercel account
- MongoDB database (You can use MongoDB Atlas for a free cloud-hosted option)

## Getting Started

1. Clone the repository:
   ```
   git clone https://github.com/nikandr-surkov/Make-TON-Telegram-Mini-App-5.git
   cd Make-TON-Telegram-Mini-App-5
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Set up your environment variables:
   Create a `.env` file in the root directory and add your MongoDB connection string:
   ```
   DATABASE_URL="your_mongodb_connection_string"
   ```

4. Generate Prisma client:
   ```
   npx prisma generate
   ```

## Deployment and Usage

As this is a Telegram Mini App, you can't see the result directly in development mode. Follow these steps to deploy and use the app:

1. Push your code to a GitHub repository.
2. Sign up for a Vercel account if you haven't already.
3. Connect your GitHub repository to Vercel and deploy the app.
4. Once deployed, Vercel will provide you with a URL for your app.
5. Use this URL to set up your Telegram Mini App:
   - Go to [@BotFather](https://t.me/BotFather) on Telegram
   - Send the command `/newapp` or choose to edit an existing bot
   - Follow the prompts to set up your Mini App, using the Vercel URL as the Web App URL
6. Once set up, you can access your Mini App through Telegram on mobile devices or in the Web version of Telegram.

## Project Structure

- `app/layout.tsx`: Root layout component with Telegram Web App script
- `app/page.tsx`: Main page component with user data handling and UI
- `app/api/user/route.ts`: API route for user creation and retrieval
- `app/api/increase-points/route.ts`: API route for increasing user points
- `prisma/schema.prisma`: Prisma schema defining the User model
- `lib/prisma.ts`: Prisma client initialization

## Key Features

- MongoDB connection using Prisma ORM
- User creation and retrieval based on Telegram data
- Points system for users
- Error handling for various scenarios
- Responsive design with Tailwind CSS

## YouTube Channel

For video tutorials and more in-depth explanations, check out my YouTube channel:
[Nikandr Surkov](https://www.youtube.com/@NikandrSurkov)

## Next Steps

Stay tuned for the next guide in the **Make TON Telegram Mini App** series, where we'll explore more advanced features and deeper integrations with the Telegram platform!