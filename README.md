## Community
- This project focuses on the development of versatile community platform 
aimed at facilitating seamless communication and collaboration among 
users from diverse communities. The platform offers a wide range of 
features including the creation of customizable channels, enabling users to 
engage in discussions, sharing resources, and collaborate on projects within 
their respective communities. Additionally, users have the flexibility to 
engage in private one-on-one chats, video calls, and audio calls, enhancing 
personal connections and fostering meaningful interactions. 

## Key Features:

- 🤯 Real-time messaging using Socket.io
- 📂 Send attachments as messages using UploadThing
- 🌐 Delete & Edit messages in real time for all users
- 🚀 Create Text, Audio and Video call Channels
- 💭 1:1 conversation between members
- 💻 1:1 video calls between members
- 🎨 Member management (Kick, Role change Guest / Moderator)
- 🔗 Unique invite link generation & full working invite system
- ♾️ Infinite loading for messages in batches of 10 (@tanstack/query)
- 📝 Server creation and customization
- 🦋 Beautiful UI using TailwindCSS and ShadcnUI
- 📆 Full responsivity and mobile UI
- 🌙 Light / Dark mode
- ⚠️ Websocket fallback: Polling with alerts 
- 🫙 ORM using Prisma
- 🦈 Postgresql database using NEON
- 👥 Authentication with Clerk

## :toolbox: Getting Started

1. Make sure **Git** and **NodeJS** is installed.
2. Clone this repository to your local computer.
3. Create `.env` file in **root** directory.
4. Contents of `.env`:

```env
# .env

# clerk auth keys
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
CLERK_SECRET_KEY=sk_test_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

# clerk redirect urls
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# neon databse url
DATABASE_URL=""

# uploading api key and app id
UPLOADTHING_SECRET=sk_live_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
UPLOADTHING_APP_ID=xxxxxxxxxxxxx

# app base url
NEXT_PUBLIC_BASE_URL=http://localhost:3000

# livekit api keys and public url
LIVEKIT_API_KEY=XXXXXXXXXXXXXXXXX
LIVEKIT_API_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
NEXT_PUBLIC_LIVEKIT_URL=

```

5. **Next.js Telemetry Disabled:**

   - Visit the Next.js documentation or repository.
   - Find the instructions to disable telemetry.
   - Set `NEXT_TELEMETRY_DISABLED` to `1` in your `.env` file.

6. **Clerk Authentication Keys:**

   - Go to the Clerk website and sign in to your account.
   - Navigate to the settings or API keys section.
   - Generate or locate your Clerk publishable and secret keys.
   - Set `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY` and `CLERK_SECRET_KEY` accordingly in the `.env` file.

7. **Clerk Redirect URLs:**

   - Refer to the Clerk documentation or settings.
   - Set the required URLs for sign-in, sign-up, after sign-in, and after sign-up.
   - Assign these URLs to `NEXT_PUBLIC_CLERK_SIGN_IN_URL`, `NEXT_PUBLIC_CLERK_SIGN_UP_URL`, `NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL`, and `NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL` respectively in the `.env` file.

8. **Neon Database URL:**

   - Access your database provider (e.g., PostgreSQL).
   - Retrieve the necessary connection details such as username, password, host, and port.
   - Construct the database URL using the obtained information and SSL mode.
   - Assign the constructed URL to `DATABASE_URL` in the `.env` file.

9. **Uploading API Key and App ID:**

   - Go to the UploadThing website or application.
   - Find the section for API keys or account settings.
   - Generate or locate your secret key and app ID.
   - Set `UPLOADTHING_SECRET` and `UPLOADTHING_APP_ID` in the `.env` file accordingly.

10. **App Base URL:**

- Determine the base URL of your application.
- Set `NEXT_PUBLIC_BASE_URL` to the base URL in the `.env` file.

11. **Livekit API Keys and Public URL:**

- Visit the Livekit website or dashboard.
- Navigate to API settings or keys section.
- Generate or locate your API key and secret.
- Set `LIVEKIT_API_KEY`, `LIVEKIT_API_SECRET`, and `NEXT_PUBLIC_LIVEKIT_URL` in the `.env` file according to the obtained information.

12. Save and Secure:

    - Save the changes to the `.env.local` file.

13. Install Project Dependencies using `npm install --legacy-peer-deps` or `yarn install --legacy-peer-deps`.

14. Now app is fully configured 👍 and you can start using this app using either one of `npm run dev` or `yarn dev`.

**NOTE:** Please make sure to keep your API keys and configuration values secure and do not expose them publicly.
