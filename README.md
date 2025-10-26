# 🧠 SmartPDF QueryBot

SmartPDF QueryBot is a simple **AI web app** that lets you **upload PDF files** and **ask questions** about their content.  
It uses **Google Gemini (Generative AI)** and **LangChain** to read, understand, and reply based on your PDFs.

---

## 🚀 Features
- Upload one or more PDFs  
- Ask questions in normal language  
- AI answers come directly from the document  
- Built with Streamlit (easy to use in the browser)  
- Uses FAISS for fast search and LangChain for processing  

---

## ⚙️ Setup Steps

### 1️⃣ Create Virtual Environment
```bash
python -m venv venv
```


---

### 2️⃣ Install Dependencies
Create a `requirements.txt` file and add:
```
streamlit
PyPDF2
faiss-cpu
chromadb
python-dotenv
langchain
langchain-text-splitters
langchain-google-genai==2.0.0
google-generativeai==0.7.2
```

Then install everything:
```bash
pip install -r requirements.txt
```

---

### 3️⃣ Add Google API Key
Create a `.env` file in your project folder and paste your key:
```
GOOGLE_API_KEY="your_api_key_here"
```
Get your key from: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

---

### 4️⃣ Run the App
```bash
streamlit run app.py
```

Then open the link shown in your terminal (like [http://localhost:8501](http://localhost:8501)).

---

## 💡 How It Works (Simple Steps)

1. You upload your PDF files.  
2. The app reads all the text using **PyPDF2**.  
3. The text is split into small parts for easy processing.  
4. Each part is converted into embeddings (numerical meaning).  
5. These embeddings are stored in **FAISS** (a vector database).  
6. You ask a question → the app searches for relevant parts in your PDF.  
7. It sends the best parts and your question to **Google Gemini AI**.  
8. Gemini generates a clear, context-based answer.  
9. You see the result instantly in the Streamlit interface.  

---

### 🔁 Summary
```
Upload PDF → Extract Text → Split → Create Embeddings
→ Store in FAISS → Ask Question → Gemini Gives Answer
```

---

## 🧩 Example
If you upload a file named `Report.pdf` and ask:

> “What is the summary of this document?”

The bot searches the file and replies with a short summary — taken directly from your PDF content.

---



---

## ✅ Conclusion
SmartPDF QueryBot makes reading PDFs easy and smart.  
It turns your documents into a chatbot using **Google Gemini**, **LangChain**, and **Streamlit**.  
Just upload, ask, and get your answers instantly.

---

**Developed by:** *Pramitha* 👩‍💻

