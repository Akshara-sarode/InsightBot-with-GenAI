## InsightBot-with-GenAI

A visually elegant, **modern GenAI-powered chatbot** that lets you **chat with your PDFs**, generate **quizzes**, **define glossary terms**, and even **talk via voice** — built using `LangChain`, `Gradio`, and `Groq LLaMA-3` model. Designed with a **Times New Roman aesthetic** and animated UI for an immersive experience.

## 🚀 Features

- 📁 **Chat with PDFs** using semantic search (vector database)
- 💬 **Conversational interface** powered by LLaMA-3 (via Groq)
- 🎙️ **Voice-to-text chat** using Whisper ASR
- 📚 **Glossary lookup** (drag-and-drop widget)
- ❓ **Quiz question generator** based on PDF content
- 📥 **Download full chat transcript**
- 🎉 Confetti, dark-mode toggle, sparkles, cursor trail, and profile pic
- 🧠 Local memory context using `LangChain` ConversationBuffer

## 🛠️ Tech Stack

- **Frontend:** Gradio (`Blocks`, custom CSS, JS injects)
- **LLM Backend:** LLaMA-3-70B via `Groq API`
- **Vector DB:** ChromaDB + `HuggingFaceBgeEmbeddings`
- **Audio/ASR:** `transformers` (`openai/whisper-tiny`)
- **PDF Parsing:** `LangChain` PyPDFLoader
- **Summarization:** T5 (`transformers` pipeline)

## 📦 Installation

```bash
pip install -q gradio langchain langchain-groq chromadb \
               sentence_transformers pdfminer.six pypdf \
               transformers sentencepiece
