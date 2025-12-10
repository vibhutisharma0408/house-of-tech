# NotesVault 📝

> **Capture. Organize. Perfect.** - Your AI-powered note-taking solution

A production-grade full-stack note-taking application with secure user authentication, complete CRUD operations, and AI-enhanced content improvement powered by OpenAI.

![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![Node](https://img.shields.io/badge/Node-18%2B-green)

---

## ✨ Features

- 🔐 **Secure Authentication** - JWT-based NextAuth with bcrypt password hashing
- 📝 **Full CRUD Operations** - Create, read, update, and delete notes seamlessly
- 🤖 **AI-Powered Enhancement** - Improve notes with OpenAI's GPT-3.5-turbo
- 🎨 **Responsive Design** - Beautiful, mobile-first UI with Tailwind CSS
- ⚡ **High Performance** - Server-side caching, optimized queries
- 🔒 **Data Privacy** - User data isolation and secure MongoDB storage
- 🌐 **Real-time Updates** - Instant note synchronization

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | Next.js 16, React 19, TypeScript |
| **Backend** | Next.js API Routes |
| **Database** | MongoDB + Mongoose |
| **Authentication** | NextAuth.js v5 with JWT |
| **Styling** | Tailwind CSS v4 |
| **AI Integration** | OpenAI API (GPT-3.5-turbo) |
| **Validation** | Zod |

---

## 📋 Prerequisites

- **Node.js** 18.0+
- **MongoDB Atlas** account (free at [mongodb.com](https://mongodb.com))
- **OpenAI API key** (get at [platform.openai.com](https://platform.openai.com/api-keys))

---

## 🚀 Quick Start

### 1. Clone Repository

```bash
git clone https://github.com/vibhutisharma0408/house-of-edtech.git
cd house-of-edtech/frontend
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create `.env.local`:

```env
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your-secret-key-here
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/notesapp
OPENAI_API_KEY=sk-proj-your-api-key-here
```

**Generate NEXTAUTH_SECRET:**
```bash
openssl rand -base64 32
```

### 4. Start Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

### 5. Create Account

1. Click "Get started"
2. Register with email/password (min 8 chars)
3. Log in and start creating notes!

---

## 📖 How to Use

### Creating a Note
1. Dashboard → "Create"
2. Enter title and content
3. Click "Create Note"

### Improving with AI
1. Open note for editing
2. Click "Improve with AI"
3. AI enhances your content

### Editing
1. Click "Edit" on note card
2. Modify and click "Update Note"

### Deleting
1. Click "Delete" on note card

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register user |
| POST | `/api/auth/signin` | Login |
| GET | `/api/notes` | Get all notes |
| POST | `/api/notes` | Create note |
| GET | `/api/notes/[id]` | Get note |
| PUT | `/api/notes/[id]` | Update note |
| DELETE | `/api/notes/[id]` | Delete note |
| POST | `/api/notes/improve` | Improve with AI |

---

## 🔐 Security

- ✅ Bcryptjs password hashing (10 rounds)
- ✅ JWT-based sessions
- ✅ User data isolation
- ✅ Input validation with Zod
- ✅ MongoDB SSL connection
- ✅ Security headers

---

## 🚀 Deployment

### Vercel (Recommended)

```bash
npm install -g vercel
vercel --prod
```

Set environment variables in Vercel Dashboard.

### Self-Hosted

```bash
npm run build
npm run start
```

---

## 📁 Project Structure

```
src/
├── app/              # Pages & API routes
├── components/       # React components
├── lib/             # Auth, DB, validation
├── models/          # MongoDB schemas
└── types/           # TypeScript definitions
```

---

## 🆘 Troubleshooting

| Issue | Solution |
|-------|----------|
| MongoDB error | Check MONGODB_URI in .env.local |
| OpenAI error | Verify API key and account credits |
| Session error | Clear cookies, log in again |
| Port in use | `lsof -ti:3000 \| xargs kill -9` |

---

## 🤝 Contributing

1. Fork repository
2. Create feature branch (`git checkout -b feature/name`)
3. Commit (`git commit -m 'Add feature'`)
4. Push (`git push origin feature/name`)
5. Open Pull Request

---

## 📝 License

MIT License

---

## 👨‍💻 Author

**Vibhuti Sharma**

- 🔗 GitHub: [@vibhutisharma0408](https://github.com/vibhutisharma0408)
- 💼 LinkedIn: [vibhuti](https://www.linkedin.com/in/vibhuti-sharma-1280b7215/)

---

<div align="center">

**Built with ❤️ by Vibhuti Sharma**

[⭐ Star this repo](https://github.com/vibhutisharma0408/house-of-edtech) if helpful!

</div>
