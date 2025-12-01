# 💼 DevTrack Backend

A backend system to help developers track tasks, goals, and productivity.  
Built with **Node.js, TypeScript, Express, PostgreSQL, and Prisma**, this project demonstrates clean backend architecture, secure authentication, task management logic, and production-ready REST APIs.

---

## 🚀 Features

### 🔐 Authentication
- JWT-based authentication (access + refresh tokens)  
- Secure password hashing with bcrypt  
- Role-based access control (user/admin)  

### 📝 Task & Project Management
- CRUD operations for tasks  
- Task status workflow (TODO → IN_PROGRESS → DONE)  
- Projects with multiple tasks  
- Priority levels (Low, Medium, High)  
- Deadlines & reminders  

### 📊 Developer Productivity
- Track daily activity logs  
- Weekly/monthly productivity stats  
- Task completion streaks  

### 🎯 Goals & Learning Tracker
- Create long-term dev goals  
- Track learning progress per topic  
- Mark progress checkpoints  

### 🗃️ Database & ORM
- PostgreSQL relational schema  
- Prisma ORM with TypeScript safety  
- Migrations & seed scripts  

### 🧩 Architecture
- Modular structure: Controller → Service → Repository  
- Zod validation  
- Global error handling middleware  
- Logger middleware  
- Environment-based configuration  

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Runtime | Node.js (TypeScript) |
| Framework | Express.js |
| Database | PostgreSQL |
| ORM | Prisma |
| Auth | JWT, bcrypt |
| Validation | Zod |
| Dev Tools | ESLint, Prettier, Nodemon, ts-node |

---

## 📁 Project Structure

```
devtrack-backend/
├── src/
│   ├── modules/
│   │   ├── auth/
│   │   ├── tasks/
│   │   ├── projects/
│   │   ├── goals/
│   │   └── analytics/
│   ├── middleware/
│   ├── utils/
│   ├── app.ts
│   └── server.ts
├── prisma/
│   ├── schema.prisma
│   └── migrations/
├── .env.example
├── package.json
└── README.md
```


---

## 🚀 Getting Started

```bash
# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Run database migrations
npx prisma migrate dev

# Start development server
npm run dev

Visit http://localhost:4000 to confirm the server is running.