# Ignite - Chat with your PDF's

## :toolbox: Getting Started

1. Make sure **Git** and **NodeJS** is installed.
2. Clone this repository to your local computer.
3. Create `.env` file in **root** directory.
4. Contents of `.env`:

```env
# .env

# disabled next.js telemetry
NEXT_TELEMETRY_DISABLED=1

# kinde keys and urls
KINDE_CLIENT_ID=XXXXXXXXXXXXXXXXXXXXXXXXXXX
KINDE_CLIENT_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
KINDE_ISSUER_URL=https://example.kinde.com
KINDE_SITE_URL=http://localhost:3000
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_POST_LOGIN_REDIRECT_URL=http://localhost:3000/dashboard

# neon db uri
DATABASE_URL="postgresql://<user>:<password>@<hostname>:<port>/quill?sslmode=require"

# uploadthing api key and app id
UPLOADTHING_SECRET=sk_live_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
UPLOADTHING_APP_ID=xxxxxxxxxxx

# app base url
NEXT_PUBLIC_BASE_URL=http://localhost:3000

# pinecone api key
PINECONE_API_KEY=xxxxxxxxxx-xxxxx-xxxx-xxxxxx-xxxxxxxxxxx

# openai api key
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

# stripe secret key, price id and webhook secret
STRIPE_SECRET_KEY=sk_test_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
STRIPE_PRICE_ID=price_XXXXXXXXXXXXXXXXXXXXXXXXX
STRIPE_WEBHOOK_SECRET=whsec_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX


```

### Kinde

- **Environment Variables**:
  - `KINDE_CLIENT_ID`
  - `KINDE_CLIENT_SECRET`
  - `KINDE_ISSUER_URL`
  - `KINDE_SITE_URL`
  - `KINDE_POST_LOGOUT_REDIRECT_URL`
  - `KINDE_POST_LOGIN_REDIRECT_URL`
- **Instructions**:
  - Visit [Kinde's website](https://example.kinde.com) and sign in to your account.
  - Navigate to your account settings or developer dashboard to find the API credentials.
  - Retrieve the following:
    - `KINDE_CLIENT_ID`
    - `KINDE_CLIENT_SECRET`
    - `KINDE_ISSUER_URL`
  - For redirect URLs:
    - `KINDE_SITE_URL`
    - `KINDE_POST_LOGOUT_REDIRECT_URL`
    - `KINDE_POST_LOGIN_REDIRECT_URL`

### Neon Database URI

- **Environment Variable**: `DATABASE_URL="postgresql://<user>:<password>@<hostname>:<port>/quill?sslmode=require"`
- **Instructions**:
  - Access your PostgreSQL database management interface.
  - Locate the database connection details.
  - Construct the URI following the provided template and replace the placeholders with your actual database credentials.

### Uploadthing

- **Environment Variables**:
  - `UPLOADTHING_SECRET`
  - `UPLOADTHING_APP_ID`
- **Instructions**:
  - Visit the Uploadthing developer dashboard or website.
  - Log in to your account and navigate to the API or application settings.
  - Retrieve `UPLOADTHING_SECRET` and `UPLOADTHING_APP_ID`.

### App Base URL

- **Environment Variable**: `NEXT_PUBLIC_BASE_URL=http://localhost:3000`
- **Instructions**:
  - Simply set `NEXT_PUBLIC_BASE_URL=http://localhost:3000` in your `.env` file.

### Pinecone API Key

- **Environment Variable**: `PINECONE_API_KEY=xxxxxxxxxx-xxxxx-xxxx-xxxxxx-xxxxxxxxxxx`
- **Instructions**:
  - Visit Pinecone's official website and log in to your account.
  - Navigate to the API or developer section to find your API key.
  - Retrieve `PINECONE_API_KEY`.

### OpenAI API Key

- **Environment Variable**: `OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`
- **Instructions**:
  - Log in to your OpenAI account on the official website.
  - Navigate to the API or developer dashboard.
  - Retrieve your API key.

### Stripe

- **Environment Variables**:
  - `STRIPE_SECRET_KEY`
  - `STRIPE_PRICE_ID`
  - `STRIPE_WEBHOOK_SECRET`
- **Instructions**:
  - Log in to your Stripe account.
  - Navigate to the API or developer section.
  - Retrieve the following:
    - `STRIPE_SECRET_KEY`
    - `STRIPE_PRICE_ID`
    - `STRIPE_WEBHOOK_SECRET`


Run `npm install` or `pnpm install` or `yarn` to install your node_modules

Now app is fully configured 👍 and you can start using this app using either one of `npm run dev` or `yarn dev` or `pnpm dev`.

And make sure to push your db to prisma `npx prisma db push` before starting.

**NOTE:** Please make sure to keep your API keys and configuration values secure and do not expose them publicly.


## :gear: Tech Stack

[![React JS](https://skillicons.dev/icons?i=react "React JS")](https://react.dev/ "React JS") [![Next JS](https://skillicons.dev/icons?i=next "Next JS")](https://nextjs.org/ "Next JS") [![Typescript](https://skillicons.dev/icons?i=ts "Typescript")](https://www.typescriptlang.org/ "Typescript") [![Tailwind CSS](https://skillicons.dev/icons?i=tailwind "Tailwind CSS")](https://tailwindcss.com/ "Tailwind CSS") [![Vercel](https://skillicons.dev/icons?i=vercel "Vercel")](https://vercel.app/ "Vercel") [![Postgresql](https://skillicons.dev/icons?i=postgres "Postgresql")](https://www.postgresql.org/ "Postgresql")



