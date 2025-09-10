# SynergySphere - Team Collaboration Platform

A modern, full-stack team collaboration platform built with **Next.js, TypeScript, Prisma, and PostgreSQL**. Manage projects, tasks, and team members with a beautiful, responsive interface.

---

## Features

### Core Functionality
- **Project Management**: Create, organize, and track team projects
- **Task Management**: Kanban-style task boards with drag-and-drop functionality
- **Team Collaboration**: Invite members, assign roles, and manage permissions
- **Real-time Notifications**: Stay updated with project and task activities
- **User Authentication**: Secure JWT-based authentication system
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile

### UI/UX Features
- **Modern Design**: Clean, intuitive interface with dark/light theme support
- **Responsive Layout**: Fully responsive design that adapts to any screen size
- **Interactive Components**: Smooth animations and hover effects
- **Accessibility**: Built with accessibility best practices
- **Custom Styling**: Tailwind CSS with custom components

---

## Tech Stack

**Frontend**
- Next.js 14 (React framework with App Router)
- TypeScript (Type-safe development)
- Tailwind CSS (Utility-first CSS framework)
- Shadcn/ui (Accessible component library)
- Lucide React (Icon library)
- Date-fns (Date manipulation utilities)

**Backend**
- Node.js (JavaScript runtime)
- Express.js (Web framework)
- Prisma (Modern ORM for database management)
- PostgreSQL (Relational database)
- JWT (JSON Web Tokens for authentication)
- Zod (Schema validation)

**Development Tools**
- ESLint (Code linting)
- Prettier (Code formatting)
- Jest (Testing framework)
- Prisma Studio (Database management UI)

---

## Quick Start

### Prerequisites
- Node.js 18+
- PostgreSQL 14+
- npm or yarn

### Installation

Clone the repository:
```bash
git clone <repository-url>
cd synergysphere
Install dependencies:

bash
Copy code
# Frontend
cd synergysphere
npm install

# Backend
cd ../backend-do
npm install
Set up the database:

bash
Copy code
# Create PostgreSQL database
createdb synergysphere

# Set up environment variables
cp .env.example .env
# Edit .env with your database credentials
Run database migrations:

bash
Copy code
cd backend-do
npx prisma migrate dev
npx prisma generate
Start the development servers:

bash
Copy code
# Terminal 1 - Backend
cd backend-do
npm run dev

# Terminal 2 - Frontend
cd synergysphere
npm run dev
Open your browser:

Frontend: http://localhost:3001

Backend API: http://localhost:3000

Prisma Studio: http://localhost:5555

Project Structure
vbnet
Copy code
synergysphere/
├── app/
│   ├── dashboard/
│   ├── auth/
│   └── globals.css
├── components/
│   ├── ui/
│   ├── auth-provider.tsx
│   ├── dashboard-layout.tsx
│   └── ...
├── lib/
│   ├── api.ts
│   └── utils.ts
└── public/

backend-do/
├── src/
│   ├── auth/
│   ├── projects/
│   ├── tasks/
│   ├── notifications/
│   ├── middleware/
│   └── lib/
├── prisma/
└── tests/
Configuration
Frontend (.env.local)

bash
Copy code
NEXT_PUBLIC_API_URL=http://localhost:3000/api/v1
Backend (.env)

ini
Copy code
DATABASE_URL="postgresql://username:password@localhost:5432/synergysphere"
JWT_SECRET="your-super-secret-jwt-key"
JWT_REFRESH_SECRET="your-super-secret-refresh-key"
NODE_ENV="development"
PORT=3000
Usage Guide
Getting Started
Register/Login

Create Project

Invite Team Members

Create Tasks

Track Progress

Key Features
Project Management

Manage multiple projects

Set project descriptions and settings

Invite team members with different roles

Track project progress and statistics

Task Management

Create tasks with titles, descriptions, and due dates

Assign tasks to team members

Organize tasks in Kanban columns (To Do, In Progress, Done)

Filter and search tasks

Team Collaboration

Invite users via email

Assign roles (Owner, Admin, Member)

Manage permissions and access levels

Real-time updates and notifications

Testing
bash
Copy code
# Backend tests
cd backend-do
npm test

# Frontend tests
cd synergysphere
npm test
Covers:

API endpoint testing

Authentication flow testing

Database operations testing

Component unit testing

Deployment
bash
Copy code
# Frontend
cd synergysphere
npm run build
npm start

# Backend
cd backend-do
npm run build
npm start
Configure PostgreSQL, environment variables, reverse proxy (nginx), SSL certificates.

Contributing
Fork the repository

Create a feature branch:

bash
Copy code
git checkout -b feature/amazing-feature
Commit your changes:

bash
Copy code
git commit -m 'Add amazing feature'
Push to your branch:

bash
Copy code
git push origin feature/amazing-feature
Open a Pull Request

Guidelines

Follow TypeScript best practices

Write meaningful commit messages

Add tests for new features

Update documentation as needed

API Documentation
Authentication Endpoints

POST /api/v1/auth/register - User registration

POST /api/v1/auth/login - User login

GET /api/v1/auth/profile - Get user profile

Project Endpoints

GET /api/v1/projects - List projects

POST /api/v1/projects - Create project

GET /api/v1/projects/:id - Get project details

PUT /api/v1/projects/:id - Update project

DELETE /api/v1/projects/:id - Delete project

Task Endpoints

GET /api/v1/tasks - List tasks

POST /api/v1/tasks - Create task

GET /api/v1/tasks/:id - Get task details

PUT /api/v1/tasks/:id - Update task

DELETE /api/v1/tasks/:id - Delete task

Troubleshooting
Database Connection Issues

Verify PostgreSQL is running

Check DATABASE_URL in .env

Ensure database exists

Authentication Issues

Check JWT_SECRET is set

Verify token expiration

Clear browser storage

Build Issues

Clear node_modules and reinstall

Check Node.js version compatibility

Verify environment variables

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Next.js

Tailwind CSS

Shadcn/ui

Prisma

Lucide

