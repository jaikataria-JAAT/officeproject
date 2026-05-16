# Team Task Manager

A full-stack Team Task Manager web application built with React, Node.js, Express, and PostgreSQL (via Prisma).

## Features
- **JWT Authentication**: Secure signup and login.
- **RBAC**: App-level and Project-level role-based access control.
- **Project Management**: Create, update, and delete projects.
- **Member Management**: Add/remove team members with specific roles.
- **Kanban Board**: Task management visualized via status columns.
- **Overdue Logic**: Automatic flags for overdue tasks.
- **Premium UI**: Modern, responsive design with Tailwind CSS.

## Tech Stack
- **Frontend**: React (Vite), Tailwind CSS, React Query, Lucide Icons.
- **Backend**: Node.js, Express, Prisma ORM, PostgreSQL.
- **Auth**: JSON Web Tokens (JWT).

## Local Setup

### Backend
1. `cd backend`
2. `npm install`
3. Create a `.env` file with `DATABASE_URL` and `JWT_SECRET`.
4. `npx prisma generate`
5. `npx prisma migrate dev`
6. `npm run dev`
7. (Optional) `node src/seed.js` to seed demo data.

### Frontend
1. `cd frontend`
2. `npm install`
3. `npm run dev`

## Deployment (Railway)
1. Link your GitHub repository to Railway.
2. Create a PostgreSQL database on Railway.
3. Configure environment variables in Railway: `DATABASE_URL`, `JWT_SECRET`.
4. Railway will automatically detect the `package.json` in each directory if you set the root directory correctly for each service.
