# 🏥 END-to-END Medical ChatBot

A complete end-to-end Generative AI–powered Medical ChatBot built using **LangChain**, **Pinecone**, **Sentence Transformers**, and **Flask**. This project provides an intelligent conversational agent capable of answering medical-related queries using vector embeddings and LLMs.

---

## 🚀 Features

* ⚕️ Medical Question Answering using LLMs
* 🔍 Semantic Search using **Sentence Transformers**
* 📚 Vector Database Integration with **Pinecone**
* 🧠 LangChain for Retrieval-Augmented Generation (RAG)
* 🌐 Simple & Fast API built with **Flask**
* 📄 PDF data ingestion using **PyPDF**
* 🔒 Environment variable handling with **dotenv**

---

## 📦 Project Structure

```
📁 END-to-END-Medical-ChatBot
│── 📁 src
│     ├── data_ingestion.py
│     ├── embeddings.py
│     ├── vector_store.py
│     ├── chat_model.py
│     └── app.py
│
│── requirements.txt
│── setup.py
│── README.md
```

---

## 🧰 Installation

### 1️⃣ Clone the repository

```
git clone https://github.com/yourusername/END-to-END-Medical-ChatBot.git
cd END-to-END-Medical-ChatBot
```

### 2️⃣ Create a virtual environment

```
python -m venv venv
source venv/bin/activate   # for Linux/Mac
venv\Scripts\activate      # for Windows
```

### 3️⃣ Install dependencies

```
pip install -r requirements.txt
```

---

## 📚 Requirements

```
sentence-transformers==2.2.2
langchain
flask
pypdf
python-dotenv
pinecone[grpc]
langchain-pinecone
langchain_community
langchain_openai
langchain_experimental
-e .
```

---

## ⚙️ Setup Instructions

### 1️⃣ Create a `.env` file

```
PINECONE_API_KEY=your_pinecone_api_key
OPENAI_API_KEY=your_openai_api_key
```

### 2️⃣ Initialize Vector Store

Run embedding script to process documents and upload vectors.

```
python src/embeddings.py
```

### 3️⃣ Start the Flask API

```
python src/app.py
```

---

## 💡 Example Query

Once server is running:

```
POST http://127.0.0.1:5000/chat
{
  "query": "What are the symptoms of diabetes?"
}
```

---

## 🛠️ Setup Script (`setup.py`)

```
from setuptools import find_packages, setup


setup(
    name='Generative AI Project',
    version='0.0.0',
    author='AI Buddies',
    author_email='alidanish.tech@gmail.com',
    packages=find_packages(),
    install_requires=[]
)
```

---

## 🤝 Contributors

👨‍💻 **AI Buddies**
📧 [alidanish.tech@gmail.com](mailto:alidanish.tech@gmail.com)

---

## 🌟 Future Enhancements

* Medical report summarization
* Symptom-based disease prediction
* Multi-language support
* Mobile UI integration

---

## 📄 License

This project is licensed under the MIT License.
