SynergySphere - Team Collaboration Platform
A modern, full-stack team collaboration platform built with Next.js, TypeScript, Prisma, and PostgreSQL. SynergySphere allows teams to manage projects, organize tasks, and collaborate seamlessly with a beautiful, responsive interface.

✨ Features
Core Functionality
Project Management - Create, organize, and track team projects from a single dashboard.

Task Management - Intuitive Kanban-style task boards with drag-and-drop functionality to visualize workflow.

Team Collaboration - Invite team members, assign custom roles (Owner, Admin, Member), and manage permissions.

Real-time Notifications - Stay updated with instant notifications for task assignments, project invitations, and key activities.

User Authentication - A secure JWT-based authentication system for user management.

Responsive Design - A single application that works seamlessly on desktop, tablet, and mobile devices.

UI/UX Features
Modern Design - A clean, intuitive interface with beautiful light and dark theme support.

Interactive Components - Smooth animations and elegant hover effects using framer-motion.

Accessibility - Built with accessibility best practices to ensure a great experience for all users.

Custom Styling - A highly customized Tailwind CSS configuration for a unique and cohesive design language.

🏗 Tech Stack
Frontend
Next.js 14 - React framework with the App Router for modern web development.

TypeScript - Ensures type-safe, maintainable, and scalable code.

Tailwind CSS - A utility-first CSS framework for rapid and consistent styling.

Shadcn/ui - A collection of beautiful, accessible, and reusable UI components.

Framer Motion - Library for smooth animations and interactive transitions.

Lucide React - A comprehensive icon library for clear visual communication.

Date-fns - A minimalist library for powerful date manipulation.

Backend
Node.js - The backend runtime environment.

Express.js - A fast, unopinionated, minimalist web framework.

Prisma - A modern and powerful ORM for database management.

PostgreSQL - A robust and reliable relational database.

JWT - JSON Web Tokens for secure and stateless authentication.

Zod - A powerful schema validation library.

Development Tools
ESLint - For enforcing code quality and consistency.

Prettier - For automatic code formatting.

Jest - For robust unit and integration testing.

Prisma Studio - A user-friendly GUI for interacting with the database.

🚀 Quick Start
Prerequisites
Before you begin, ensure you have the following installed on your machine:

Node.js (version 18 or higher)

PostgreSQL (version 14 or higher)

npm or yarn

Installation
Clone the repository:

Bash

git clone https://github.com/your-username/synergysphere.git
cd synergysphere
Install dependencies:

Bash

# Install frontend dependencies
npm install

# Install backend dependencies
cd backend-do
npm install
Set up the database:

Bash

# Create the PostgreSQL database
createdb synergysphere

# Navigate back to the backend directory and set up environment variables
cp .env.example .env
Edit the .env file in the backend-do directory with your database credentials and a secret key:

DATABASE_URL="postgresql://username:password@localhost:5432/synergysphere"
JWT_SECRET="your-super-secret-jwt-key"
JWT_REFRESH_SECRET="your-super-secret-refresh-key"
NODE_ENV="development"
PORT=3000
Run database migrations:

Bash

# In the backend-do directory
npx prisma migrate dev
npx prisma generate
Start the development servers:
Open two separate terminal windows.

Terminal 1 (Backend):

Bash

cd backend-do
npm run dev
Terminal 2 (Frontend):

Bash

cd synergysphere
npm run dev
Open your browser
The application will now be running on your local machine.

Frontend: http://localhost:3001

Backend API: http://localhost:3000/api/v1

Prisma Studio: http://localhost:5555

📂 Project Structure
synergysphere/
├── app/                    # Next.js App Router pages
│   ├── dashboard/          # Dashboard & project management pages
│   ├── auth/               # User authentication pages (login, register)
│   └── globals.css         # Global styles & Tailwind directives
├── components/           # Reusable UI components
│   ├── ui/               # Shadcn/ui base components
│   ├── auth-provider.tsx # Authentication context provider
│   ├── dashboard-layout.tsx# Main application layout
│   └── ...                 # Feature-specific components
├── lib/                  # Utility functions
│   ├── api.ts            # Frontend API client
│   └── utils.ts          # General helper functions
├── public/               # Static assets (images, fonts, etc.)
└── ...

backend-do/
├── src/
│   ├── auth/             # Authentication routes, controllers, and services
│   ├── projects/         # Project management logic
│   ├── tasks/            # Task management logic
│   ├── notifications/    # Notification system logic
│   ├── middleware/       # Express middleware (e.g., authentication)
│   └── lib/              # Database connection & other utilities
├── prisma/               # Prisma database schema & migrations
├── tests/                # Jest test files
└── ...
📝 Usage Guide
Getting Started
Register/Login: Create a new account or sign in with existing credentials.

Create Project: Start by creating your first project and giving it a name and description.

Invite Team Members: Add your team members to the project via their email addresses.

Create Tasks: Break down your work into manageable tasks and assign them to team members.

Track Progress: Use the Kanban board to track the status of tasks as they move from "To Do" to "In Progress" and "Done."

🧪 Testing
Running Tests
To run the test suite for the backend:

Bash

cd backend-do
npm test
Test Coverage
API endpoint testing

Authentication flow testing

Database operations testing

Component unit testing

🤝 Contributing
We welcome contributions! Please follow these steps to contribute to the project:

Fork the repository.

Create a new feature branch (git checkout -b feature/your-feature-name).

Commit your changes (git commit -m 'feat: Add your new feature').

Push to the branch (git push origin feature/your-feature-name).

Open a Pull Request with a clear description of your changes.

Development Guidelines
Follow TypeScript best practices.

Write meaningful and descriptive commit messages.

Ensure all new features include corresponding tests.

Keep documentation up to date with any changes.

📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.

🙏 Acknowledgments
Next.js for the amazing React framework.

Tailwind CSS for the utility-first CSS approach.

Shadcn/ui for the beautiful and accessible component library.

Prisma for the modern and intuitive ORM.

Lucide for the fantastic icon library.

Built with ❤️ by the SynergySphere Team.
