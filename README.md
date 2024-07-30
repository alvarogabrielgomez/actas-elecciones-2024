# Actas Elecciones 2024

# FORKEALO, pero usa cache por favor !!!

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [Deployment](#deployment)
- [Contributing](#contributing)

## Features

- Consultation of voting information by cédula
- Display of personal voting details
- Viewing of acta (voting record) image when available
- Error handling for API request failures
- Caching with Supabase 

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js (v14.0.0 or later)
- npm (v6.0.0 or later)
- A Supabase database

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/ielijose/actas-elecciones-2024.git
   cd actas-elecciones-2024
   ```

2. Install the dependencies:
   ```
   npm install
   ```

## Configuration

1. Create a `.env.local` file in the root directory of the project.

2. Add the following environment variables to the `.env.local` file:

   ```
   NEXT_PUBLIC_SUPABASE_URL=
   SUPABASE_SERVICE_ROLE_KEY=
   ```

   Replace varaibles with your actual Supabase credentials.

## Running the Application

To run the application in development mode:

```
npm run dev
```

The application will be available at `http://localhost:3000`.

## Deployment

This application is designed to be deployed on Vercel, but you can deploy it to any platform that supports Next.js applications.

### Deploying to Vercel

1. Push your code to a GitHub repository.

2. Go to [Vercel](https://vercel.com) and sign up or log in.

3. Click on "Import Project" and select your GitHub repository.

4. Configure your project settings:

   - Framework Preset: Next.js
   - Build Command: `npm run build`
   - Output Directory: `.next`

5. Add your environment variables in the Vercel project settings.

6. Click "Deploy" and wait for the deployment to complete.

### Deploying to Other Platforms

For other platforms, consult their specific documentation for deploying Next.js applications. Generally, you'll need to:

1. Build the application:

   ```
   npm run build
   ```

2. Start the application in production mode:
   ```
   npm start
   ```

Ensure that you set up your environment variables on your hosting platform.

## Contributing

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-branch-name`.
5. Create a pull request.
