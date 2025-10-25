# Smartpdf-QueryBot
A PDF-based chatbot for querying documents using AI
📚 SmartPDF QueryBot — Chat with PDF using Gemini

SmartPDF QueryBot allows you to chat with your PDF documents using natural language.
You can upload multiple PDFs and ask questions — the app will extract answers directly from the content using Google Gemini AI.

⭐ Features

Upload and process multiple PDFs

Automatically extracts text from PDF pages

Splits text into manageable chunks for accurate results

Embedding generation using Gemini AI

FAISS vector search for fast similarity lookup

Context-aware answers based on PDF content

Simple and interactive Streamlit UI

🛠 Tech Stack
Purpose	Technology Used
UI Framework	Streamlit
Language Model & Embeddings	Google Gemini
Text Extraction	PyPDF2
Vector Database	FAISS
Text Chunking Pipeline	LangChain
Environment Variables	python-dotenv
🚀 Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/Pramithack/Smartpdf-QueryBot.git
cd Smartpdf-QueryBot

2️⃣ Install the required dependencies
pip install -r requirements.txt

3️⃣ Set up the Google API Key

Create a .env file in the project folder and add:

GOOGLE_API_KEY=your_api_key_here


Get your API Key from:
https://aistudio.google.com/app/apikey

4️⃣ Run the application
streamlit run app.py



🧠 How It Works

1️⃣ Upload one or more PDFs
2️⃣ Extract text from each page
3️⃣ Convert into chunks using LangChain
4️⃣ Generate embeddings via Gemini
5️⃣ Store embeddings in FAISS
6️⃣ Ask questions — bot fetches relevant chunk & responds intelligently
