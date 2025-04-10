# url-shortner-project
---

```markdown
# 🔗 URL Shortener Web Service using FastAPI

This project implements a simple URL shortening service using FastAPI and SQLite. It allows users to shorten long URLs and access the original links using the generated short codes. The project runs locally and can be accessed through a public link via Ngrok.

---

## 🚀 Features

- Shorten any valid URL with a single API call.
- Retrieve original URL using the short code.
- SQLite database for persistent storage.
- FastAPI backend served using Uvicorn.
- Ngrok tunneling for public access from local machine.

---

## 🛠️ Technologies Used

- Python 3
- FastAPI
- Uvicorn
- SQLAlchemy
- SQLite
- Pyngrok
- Requests
- shortuuid

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd <your-repo-name>
```

### 2. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\\Scripts\\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

## 🧪 How to Run

```bash
python app.py
```

This will:

- Start the FastAPI app locally on port 8001.
- Establish an Ngrok tunnel to make your app accessible publicly.
- Show a sample response with a shortened URL.

---

## 🧪 API Endpoints

### 🔸 POST /shorten

- **Description**: Accepts a long URL and returns a shortened version.
- **Request Body**:
```json
{
  "original_url": "https://example.com"
}
```
- **Response**:
```json
{
  "short_url": "https://<ngrok-url>/<short_code>"
}
```

---

### 🔹 GET /{short_code}

- **Description**: Redirects or fetches the original long URL from the given short code.
- **Response**:
```json
{
  "message": "Redirect",
  "original_url": "https://example.com"
}
```

---

## 🖼️ Screenshots

Demo screenshots are available in the `screenshots/` directory, covering:

- App running in terminal
- Ngrok public link
- POST /shorten response
- GET /<short_code> usage

---

## ✅ Assignment Task Checklist

- [x] Built a FastAPI service for URL shortening ✅  
- [x] Connected with SQLite DB for storing URLs ✅  
- [x] Used Ngrok to make local server public ✅  
- [x] Demonstrated API calls and responses ✅  
- [x] Requirements file generated ✅  
- [x] Screenshots included ✅  
- [x] README file complete ✅  

---

## 📬 Contact

For any queries, feel free to reach out!
```

---

Let me know once you’ve done this or if you’d like help with the next step!
