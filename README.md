# 🇵🇰 PakLegalAI – AI-Powered Pakistani Legal Assistance Chatbot

**PakLegalAI** is an AI-powered legal assistance chatbot designed to make Pakistani legal information more accessible and understandable. It helps users explore legal information across Family, Property, and Criminal Law through an interactive conversational interface.

The system combines Natural Language Processing (NLP), Large Language Models (LLMs), and Retrieval-Augmented Generation (RAG) to provide context-aware responses grounded in Pakistani legal documents and legal question-answering data.

## 🎯 Project Objectives

- Make Pakistani legal information accessible to the general public.
- Simplify complex legal terminology through conversational AI.
- Provide information across Family, Property, and Criminal Law.
- Retrieve relevant legal information from a curated knowledge base.
- Reduce the difficulty of finding and understanding relevant legal provisions.

## ✨ Key Features

- **AI-Powered Legal Chatbot:** Interact with the system using natural language.
- **Retrieval-Augmented Generation (RAG):** Retrieve relevant legal context before generating responses.
- **Multiple Legal Domains:** Supports Family, Property, and Criminal Law.
- **Legal Query Classification:** Distinguishes legal queries from non-legal queries.
- **Semantic Search:** Uses vector-based retrieval to identify relevant legal information.
- **User Authentication:** Supports Google, GitHub, and email-based login.
- **Chat Management:** Allows users to rename and delete conversations.
- **Privacy and Terms:** Includes dedicated privacy and terms information.

## 🏗️ System Architecture

PakLegalAI follows a modular architecture consisting of a frontend, backend, database, and AI-powered retrieval and generation components.

### Architecture Workflow

1. **User Input:** The user submits a legal question through the React frontend.
2. **Query Classification:** The system identifies whether the submitted question is relevant to the legal domain.
3. **Legal Information Retrieval:** FAISS retrieves relevant information from the indexed legal knowledge base.
4. **Context Preparation:** Retrieved legal information is prepared as context for the language model.
5. **Response Generation:** LLaMA 3.2 generates a contextual response using the retrieved information.
6. **Response Delivery:** The generated response is returned to the frontend and displayed to the user.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | React.js |
| Backend | FastAPI |
| Database | MongoDB |
| Large Language Model | LLaMA 3.2 |
| AI Model Platform | Hugging Face |
| Vector Database / Search | FAISS |
| NLP | Transformer-based models |
| Programming Language | Python, JavaScript |

## 📚 Legal Knowledge Base

The system uses a curated legal knowledge base developed from Pakistani legal resources.

The knowledge base includes:

- Family Law
- Property Law
- Criminal Law
- Legal question-and-answer data

The project involved processing nine legal PDF documents into structured CSV datasets to support information retrieval.

A legal question-answering dataset containing approximately 100 records was also prepared and divided into training and testing subsets.

Additionally, an approximately 8,000-record dataset was developed for legal and non-legal query classification.

## 🧠 AI and Machine Learning

The project incorporates multiple AI and NLP techniques:

- **Large Language Models:** LLaMA 3.2 for contextual response generation.
- **Retrieval-Augmented Generation:** Combines document retrieval with language generation.
- **Vector Search:** FAISS for efficient similarity-based retrieval.
- **Text Classification:** Transformer-based approaches for identifying legal and non-legal queries.
- **Data Preprocessing:** Document extraction, cleaning, structuring, and preparation for retrieval and model training.

## 📁 Project Structure

```text
Pak-Legal-AI/
│
├── Backend/
│   └── Backend source code and API implementation
│
├── Frontend/
│   └── React application and user interface
│
├── .gitignore
│
└── README.md
```

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or compatible version
- Node.js and npm
- MongoDB
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/Umair-Ahmed786/Pak-Legal-AI.git

cd Pak-Legal-AI
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd Backend
```

Install the dependencies using the project's requirements file, if provided:

```bash
pip install -r requirements.txt
```

Configure the required environment variables for MongoDB and AI model access.

Start the FastAPI application using the project's configured entry point.

### 3. Frontend Setup

Navigate to the frontend directory:

```bash
cd Frontend
```

Install dependencies:

```bash
npm install
```

Start the development server using:

```bash
npm run dev
```


## ⚠️ Disclaimer

PakLegalAI is an educational and informational project. It provides AI-generated legal information for awareness purposes and does not replace professional legal advice. Users should consult qualified legal professionals for advice concerning specific legal matters.

## 👩‍💻 Contributors

Developed as an academic Final Year Project at **Sukkur IBA University**.
