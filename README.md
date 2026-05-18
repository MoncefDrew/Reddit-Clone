# Breaddit

A Reddit-style community platform built with Next.js, Prisma, and MySQL. Users can create communities, post content, vote, comment, and manage their profiles — all in a responsive, real-time interface.

---

## Features

- **Authentication** — Login and registration via NextAuth.js with Google OAuth
- **Communities** — Create, join, and manage subreddit-style groups with custom rules
- **Posts & Comments** — Rich text posts with nested comments and upvote/downvote support
- **Real-time Updates** — Live vote counts and post activity powered by Redis caching
- **Profile Customization** — Users can personalize their public profiles
- **Responsive Design** — Optimized for desktop and mobile with Tailwind CSS

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js 14, React, Tailwind CSS |
| Backend | Next.js API Routes, Prisma ORM |
| Database | MySQL (via Railway) |
| Auth | NextAuth.js (Google Provider) |
| Caching | Redis |
| File Uploads | UploadThing |

---

## Getting Started

### Prerequisites

- Node.js 18+
- A MySQL database (e.g. [Railway](https://railway.app))
- A Redis instance
- Google OAuth credentials
- An [UploadThing](https://uploadthing.com) account

### Installation

```bash
git clone https://github.com/MoncefDrew/Breaddit.git
cd Breaddit
npm install
```

### Environment Variables

Create a `.env` file at the root of the project:

```env
DATABASE_URL=

NEXTAUTH_SECRET=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=

UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

REDIS_URL=
```

### Run the App

```bash
# Push the database schema
npx prisma db push

# Start the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Screenshots

![Home feed](https://raw.githubusercontent.com/MoncefDrew/Breaddit/Master/public/Screenshot%20from%202025-05-04%2023-12-14.png)

![Community page](https://raw.githubusercontent.com/MoncefDrew/Breaddit/Master/public/Screenshot%20from%202025-05-04%2023-14-22.png)

![Post view](https://raw.githubusercontent.com/MoncefDrew/Breaddit/Master/public/Screenshot%20from%202025-05-04%2023-14-40.png)

![Comments](https://raw.githubusercontent.com/MoncefDrew/Breaddit/Master/public/Screenshot%20from%202025-05-04%2023-14-52.png)

![Profile](https://raw.githubusercontent.com/MoncefDrew/Breaddit/Master/public/Screenshot%20from%202025-05-04%2023-15-13.png)

---

## License

MIT — free to use and modify.
