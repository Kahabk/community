# Orbit Community Chat

A learning-focused full-stack community chat application.

## Features

- Email/password registration and login
- Automatically generated user profiles
- PostgreSQL database
- Community rooms
- Real-time messages
- Responsive desktop/mobile interface
- Message deletion by owner
- Row Level Security policies

## Stack

- React
- TypeScript
- Vite
- Supabase Auth
- Supabase PostgreSQL
- Supabase Realtime

## 1. Create the frontend

```bash
npm install
```

## 2. Create Supabase project

1. Create a project in Supabase.
2. Open SQL Editor.
3. Paste and run `supabase/schema.sql`.
4. Open Project Settings / API or the Connect dialog.
5. Copy your Project URL and anon/publishable key.

## 3. Configure environment variables

```bash
cp .env.example .env
```

Edit `.env`:

```env
VITE_SUPABASE_URL=https://YOUR_PROJECT.supabase.co
VITE_SUPABASE_ANON_KEY=YOUR_KEY
```

Never place the Supabase service-role key in the browser application.

## 4. Run the app

```bash
npm run dev
```

Open the URL printed by Vite.

## Study order

1. `src/main.tsx` â React entry point
2. `src/App.tsx` â application state and data loading
3. `src/components/Auth.tsx` â forms and authentication
4. `src/components/Sidebar.tsx` â room creation and list rendering
5. `src/components/Chat.tsx` â database queries and realtime
6. `supabase/schema.sql` â tables, constraints, triggers and security
7. `src/styles.css` â responsive application layout

## Next features to build

- Edit profile and upload avatar
- Private/direct messages
- Room membership and private rooms
- Typing indicators
- Presence and true online status
- Image/file uploads
- Reactions and message replies
- Admin dashboard and moderation
- Notifications
- Search and pagination
