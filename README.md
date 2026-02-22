# 🤖 Responsive Chatbot API

A scalable and intelligent AI-powered chatbot backend built using
FastAPI, LangChain, and Groq LLM, with MongoDB for conversation storage
and memory management.

------------------------------------------------------------------------

## 📌 Project Overview

Responsive Chatbot is designed to serve as a backend engine for AI chat
applications.\
It integrates a Large Language Model (LLM) through Groq using LangChain
and stores chat interactions in MongoDB for persistent memory.

This makes it suitable for:

-   AI chat applications\
-   Customer support bots\
-   Personal AI assistants\
-   Web or mobile chatbot systems\
-   Internal organization chat tools

------------------------------------------------------------------------

## 🚀 Features

-   ⚡ FastAPI-based REST API\
-   🧠 Groq LLM integration via LangChain\
-   🗄 MongoDB-based chat history storage\
-   🔁 Context-aware conversation support\
-   🌐 CORS enabled (frontend ready)\
-   🔐 Secure environment variable configuration\
-   📄 Interactive Swagger API documentation

------------------------------------------------------------------------

## 🛠 Tech Stack

-   Backend: FastAPI\
-   LLM Integration: LangChain + Groq\
-   Database: MongoDB\
-   Server: Uvicorn\
-   Environment Management: python-dotenv

------------------------------------------------------------------------

## 📁 Project Structure

Responsive_chatbot/ │ ├── app.py \# Main FastAPI application ├──
requirements.txt \# Project dependencies ├── .env \# Environment
variables (not pushed to GitHub) └── README.md \# Project documentation

------------------------------------------------------------------------

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

git clone https://github.com/sudhakargovindasamy/Responsive_chatbot.git
cd Responsive_chatbot

### 2️⃣ Create Virtual Environment

python -m venv venv

Activate:

Windows: venv`\Scripts`{=tex}`\activate`{=tex}

Mac/Linux: source venv/bin/activate

### 3️⃣ Install Dependencies

pip install -r requirements.txt

------------------------------------------------------------------------

## 🔐 Environment Variables

Create a .env file in the root directory and add:

GROQ_API_KEY=your_groq_api_key_here
MONGODB_URI=your_mongodb_connection_string

------------------------------------------------------------------------

## ▶️ Running the Application

uvicorn app:app --reload

Server will run at: http://127.0.0.1:9000

API Docs: http://127.0.0.1:9000/docs

Live API: https://responsive-chatbot-yl1o.onrender.com/

------------------------------------------------------------------------

## 📡 API Endpoints

### GET /

Returns a welcome message.

### POST /chat

Request Body: { "user_id": "user1", "question": "Hello!" }

Response: { "response": "Hello! How can I assist you today?" }

------------------------------------------------------------------------

## 🗄 Database Design

Each chat interaction stores: - user_id - role (user / assistant) -
message - timestamp

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Frontend UI integration (React / Next.js)\
-   Authentication & user session management\
-   Streaming responses\
-   Docker containerization\
-   Cloud deployment

------------------------------------------------------------------------

## 👨‍💻 Author

Sudhakar G\
CSE -- Artificial Intelligence & Machine Learning

------------------------------------------------------------------------

## 📜 License

This project is open-source and available for educational and
development purposes.
