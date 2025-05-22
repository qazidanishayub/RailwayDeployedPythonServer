# 🧠 LinkedIn Post Generator API (Gemini + FastAPI)

This is a backend API built with **FastAPI** that generates professional LinkedIn posts using **Google Gemini 1.5 Pro** via the `google-generativeai` SDK. It is designed to work with a frontend like React or Next.js and deploys easily on **Railway**.

---

## 🚀 Features
- Uses Google Gemini 1.5 Pro model for advanced text generation
- Accepts user input and domain to personalize the content
- Returns fully structured LinkedIn-ready posts
- CORS enabled for frontend interaction
- Ready for Railway deployment

---

## 📂 Project Structure

```
.
├── generate.py          # FastAPI app with /generate endpoint
├── requirements.txt     # Python dependencies
├── Procfile             # For Railway deployment
└── README.md            # You’re here!
```

---

## 🧪 Local Setup

1. Clone the repo:
```bash
git clone https://github.com/yourusername/linkedin-post-generator-api
cd linkedin-post-generator-api
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set your environment key:
```bash
export GEMINI_API_KEY=your_google_api_key_here
```

4. Run the server:
```bash
uvicorn generate:app --reload
```

---

## 🌐 Endpoint

**POST** `/generate`

**Payload** (JSON):
```json
{
  "user_idea": "Using RAG with LangChain and Pinecone",
  "domain": "AI/ML/GenAI"
}
```

**Response**:
```json
{
  "post": "✅ Your generated LinkedIn post here..."
}
```

---

## 🚀 Deploy on Railway

1. Push your code to a GitHub repo.
2. Go to [https://railway.app](https://railway.app)
3. Create new project → Deploy from GitHub.
4. Add `GEMINI_API_KEY` as an environment variable.
5. Deploy! 🎉

You’ll get a URL like:
```
https://your-app-name.up.railway.app/generate
```

---

## 🛠 Built With
- FastAPI
- Google Generative AI (Gemini 1.5 Pro)
- Railway

---

## 🧑‍💻 Author
Qazi Danish — [linkedin.com/in/qazidanish](https://linkedin.com/in/qazidanish)