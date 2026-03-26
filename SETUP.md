# ZXNV AI - Backend Setup Guide

## ✅ Using OpenRouter.ai

Your app is now using **OpenRouter.ai** for API calls (via a secure backend server). This:
- ✅ Supports multiple AI models (Claude, GPT-4, Mistral, etc.)
- ✅ Hides your API key (not exposed in browser)
- ✅ Better rate limit handling & more affordable
- ✅ More professional/production-ready

---

## 🚀 Setup Instructions

### Step 1: Install Node.js
Download & install from: https://nodejs.org/ (LTS version recommended)

### Step 2: Navigate to Your Project
```powershell
cd "C:\Users\ASUS\Documents\ZXNV AI"
```

### Step 3: Install Dependencies
```powershell
npm install
```

### Step 4: Your API Key is Already Set!
Your OpenRouter API key is already configured in the `.env` file:
```
OPENAI_API_KEY=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
```

**📌 IMPORTANT**: 
- Your API key stays **only on your server** (never sent to browser)
- It's safe as long as you keep `.env` file private
- Don't commit `.env` to git/github

### Step 5: Start the Server
```powershell
npm start
```

You should see:
```
🚀 ZXNV AI Server running on http://localhost:3000
📝 Make sure .env file exists with OpenRouter API key
🌐 Open http://localhost:3000 in your browser
```

### Step 6: Open the App
Open your browser to: **http://localhost:3000**

---

## 🧪 Testing Your Setup

Once the server is running:

1. Open http://localhost:3000 in browser
2. Log in with any username
3. Try sending a message
4. If it works, you're all set! ✅

---

## 🧪 Testing the API

Once the server is running:

1. Open http://localhost:3000 in browser
2. Log in with any username
3. Try sending a message
4. If it works, you're all set! ✅

---

## ❌ Troubleshooting

### "Cannot find module 'express'"
→ Run: `npm install`

### "API key not configured on server"
→ Check `.env` file has your OpenRouter API key

### "Still getting 429 error"
→ Your OpenRouter account needs:
  - Valid API key (should be working now!)
  - Check: https://openrouter.ai

### "Connection refused on localhost:3000"
→ Make sure server is running: `npm start`

### "Cannot GET /"
→ Server should be running. Try closing (Ctrl+C) and restarting: `npm start`

---

## 📝 File Structure
```
ZXNV AI/
├── ai.html          (Your app - open in browser)
├── server.js        (Backend proxy - handles OpenRouter API calls)
├── .env             (Your OpenRouter API key - KEEP PRIVATE!)
├── package.json     (Dependencies list)
└── SETUP.md         (This file)
```

---

## 🔒 Security Notes

✅ **DO:**
- Keep `.env` file private on your computer
- Never share your API key
- Don't upload `.env` to GitHub

❌ **DON'T:**
- Put API keys in HTML/JavaScript files
- Commit `.env` to version control
- Share your API key publicly

---

Good luck! 🚀
