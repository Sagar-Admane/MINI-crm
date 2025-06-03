🚀 AI-Powered CRM – Xeno SDE Internship Assignment
This is my submission for the Xeno SDE Internship Assignment 2025.
It’s a full-stack CRM platform with AI-powered campaign strategy, real-time audience segmentation, Google OAuth, Redis stream processing, and campaign communication logs — all built for performance and clarity.

🔗 Live Links
🌐 Frontend (Vercel): [https://your-vercel-app.vercel.app](https://crm-frontend-sage.vercel.app/)

⚙️ Backend (Render): [https://your-backend.onrender.com](https://mini-crm-backend-zamw.onrender.com)

🎥 Demo GIF (Recommended)
Include a GIF or Loom video showing:

Login with Google

Creating a customer

Creating a campaign

Using AI message suggestions

Viewing campaign logs

✨ Features
🔐 Google OAuth login via Passport.js

🧠 AI-Powered campaign strategies using OpenAI GPT-3.5

📬 AI-generated SMS/email message suggestions

🎯 Rule-based audience segmentation

📊 Campaign creation and delivery tracking

🔁 Redis Streams for customer ingestion and async processing

📝 Communication logs per customer

👁️ View logs per campaign in a clean UI

💾 MongoDB persistence with campaign + user linkage

⚡️ Fully deployed on Vercel + Render

⚙️ Tech Stack
Layer	Tech
Frontend	React, Vite, TailwindCSS
Backend	Node.js, Express.js
Database	MongoDB (with Mongoose)
AI	OpenAI GPT-3.5 Turbo
Auth	Google OAuth 2.0 + Passport.js
Queue	Redis Streams + ioredis
Hosting	Vercel (FE), Render (BE)

🔄 Application Workflow
plaintext
Copy
Edit
[Login with Google]
       ↓
[Dashboard] —> [Create Customer] → Redis Stream → MongoDB
     ↓
[Build Campaign]
     ↓
Select Rules → Preview Audience → AI Message Suggestion → Send → Save to DB
     ↓
[View History]
     ↓
View Logs (Success / Failed)
🤖 AI Features
Feature	Description
Message Generator	Generates SMS/email content from campaign goals
Strategy Builder	Builds full re-engagement plans from a single prompt
Bonus	Suggests human-like content for inactive users

🛠️ Setup (Local)
🔧 Backend
bash
Copy
Edit
cd crm-backend
npm install
npm run dev
Add .env file:

env
Copy
Edit
PORT=3001
GOOGLE_CLIENT_ID=...
GOOGLE_CLIENT_SECRET=...
SESSION_SECRET=your-secret
MONGODB_URI=...
OPENAI_API_KEY=sk-xxx
🖼 Frontend
bash
Copy
Edit
cd crm-frontend
npm install
npm run dev
Add .env:

env
Copy
Edit
VITE_API_BASE_URL=http://localhost:3001
🧠 AI Prompt Examples
txt
Copy
Edit
"Create a strategy to re-engage users who haven’t ordered in 3 months"
"Suggest 3 SMS messages to bring back inactive users"
📂 Folder Structure
bash
Copy
Edit
crm-backend/
├── models/
├── routes/
├── controllers/
├── workers/    # Redis stream consumer
├── auth/       # Passport strategy
└── index.js

crm-frontend/
├── pages/
│   ├── CampaignBuilder.jsx
│   ├── CampaignHistory.jsx
│   ├── StrategyBuilder.jsx
│   └── MessageSuggester.jsx
└── main.jsx
✅ Completed Phases
Phase	Feature
1	Customer ingestion (Redis Stream → MongoDB)
2	Campaign Builder + Rule engine
3	Message simulation + logs
4	Communication log tracking
5	Google OAuth 2.0 integration
6	AI Integration (OpenAI)

🧪 Future Improvements
Role-based access for marketers/admins

Campaign scheduling with cron jobs

Dashboard analytics & visualization

Product recommendations via vector embeddings

Real notification system

👨‍💻 Author
Sagar Admane
🎓 B.Tech Student – Full Stack + AI
🔗 LinkedIn
🌐 Portfolio
