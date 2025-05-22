# LinkedIn AI Post Generator (Frontend + Gemini API)

This project is a two-part AI-powered LinkedIn content generator. The **frontend** is built with Next.js and hosted on Vercel, while the **backend** is a FastAPI application powered by Gemini (Google Generative AI), deployed via Render.

---

## 🌐 Live Deployment Structure

```
/frontend (Next.js app on Vercel)
/api/generate.py (FastAPI Gemini API on Render)
```

---

## 🚀 Features

- Custom or AI-generated prompts for LinkedIn posts
- Supports domains like AI/ML, SaaS, GenAI, Agentic AI, etc.
- FastAPI backend using Gemini 1.5 Pro
- Copy-ready LinkedIn post formatting
- CORS-enabled API for cross-domain requests

---

## 📦 Backend Setup (Render)

1. Clone this repo or move `generate.py` and `requirements.txt` to a separate repo.
2. Go to [Render.com](https://render.com) and create a **New Web Service**
3. Set up with the following:
   - **Start Command**: `uvicorn generate:app --host 0.0.0.0 --port 10000`
   - **Build Command**: `pip install -r requirements.txt`
   - **Port**: `10000`
   - **Environment Variable**: `GEMINI_API_KEY`

---

## 💻 Frontend Setup (Vercel)

1. Deploy `/frontend` as a Next.js app to Vercel.
2. In your `index.tsx` or wherever you fetch the post:
   ```ts
   fetch("https://your-render-api-url.onrender.com/generate", { ... })
   ```
3. Add environment variable `GEMINI_API_KEY` to Vercel (optional if you proxy request)

---

## 📄 Tech Stack

- FastAPI
- Google GenerativeAI (`gemini-1.5-pro-001`)
- Next.js (React 18+)
- Tailwind (optional for UI)
- Render (backend)
- Vercel (frontend)

---

## 📬 Contact

Built by Qazi Danish  
For technical support or questions, message on [LinkedIn](https://www.linkedin.com).