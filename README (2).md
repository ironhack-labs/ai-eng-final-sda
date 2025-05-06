# 🚀 YouTube Medical Assistant: Smart Medical Q\&A System with Whisper, LangChain, and ChromaDB

This project builds a **full-stack Medical QA Assistant** that:

* 🧠 Ingests medical educational YouTube videos (e.g., blood pressure, CPR, diabetes)
* 🎤 Transcribes audio using **OpenAI Whisper**
* 📚 Stores knowledge chunks in a **Chroma vector database**
* 🔎 Answers user questions using **retrieval-augmented generation (RAG)** powered by **OpenAI GPT**
* 🎛️ Offers an interactive **Gradio web interface** for text and voice queries
* 📊 Supports **LangSmith evaluation** and generates full **performance visualizations**

---

## 📚 Project Overview

* ✅ Download medical YouTube videos (audio-focused)
* 📝 Transcribe audio to text with OpenAI **Whisper**
* ✂️ Split text into meaningful chunks
* 🧠 Embed and store knowledge in **ChromaDB** vector database
* 🔁 Retrieve relevant context for questions
* 🤖 Generate answers using **ChatGPT** (`gpt-3.5-turbo`)
* 🎛️ Provide a **Gradio UI** for users to ask via typing or microphone
* 🧪 Evaluate model accuracy, latency, and uncertainty using **LangSmith**
* 📈 Visualize system architecture, workflows, performance dashboards, and knowledge graphs

---

## 🛠️ Tech Stack

| Component             | Tool/Library                                  |
| --------------------- | --------------------------------------------- |
| Video Download        | `yt-dlp`                                      |
| Speech-to-Text        | `whisper` (OpenAI)                            |
| Text Embedding        | `sentence-transformers` / `OpenAI Embeddings` |
| Vector Store          | `ChromaDB` + `langchain_community`            |
| LLM / QA              | `langchain-openai` (ChatOpenAI)               |
| UI Interface          | `Gradio`                                      |
| Evaluation/Monitoring | `LangSmith`                                   |
| Visualization         | `matplotlib`, `seaborn`, `networkx`           |
| Environment           | Google Colab / Jupyter                        |

---

## 🧪 How It Works

1. 📥 Download YouTube medical videos (audio only)
2. 🎤 Transcribe speech to text with Whisper
3. ✂️ Split transcripts into overlapping chunks
4. 🧠 Store chunks as vector embeddings in **Chroma**
5. 🧠 Retrieve top relevant chunks when user asks a question
6. 🤖 Use **GPT-3.5-turbo** to generate answers based on retrieved context
7. 🎛️ Interact via Gradio (text box or microphone)
8. 📈 Evaluate system performance with **LangSmith** and visualizations

---

## 💻 Notebook / Code Contents

* `YouTube_Medical_Assistant.ipynb`

  * [x] Install packages and set up API keys
  * [x] Download YouTube videos and extract audio
  * [x] Transcribe audio using OpenAI Whisper
  * [x] Store transcripts in Chroma vector database
  * [x] Build Retrieval-Augmented QA system
  * [x] Develop Gradio web app (text + voice input)
  * [x] Run LangSmith evaluation on test questions
  * [x] Generate system architecture diagrams, workflows, dashboards, and knowledge graphs

---

## 🧠 Example Test Questions

| Question                                          | Response Accuracy |
| ------------------------------------------------- | ----------------- |
| What is considered a high blood pressure reading? | ✅                 |
| What is the first step when performing CPR?       | ✅                 |
| How does type 1 diabetes differ from type 2?      | ✅                 |
| Can stress cause high blood pressure?             | ✅                 |
| Is mouth-to-mouth necessary for CPR?              | ✅                 |
| What dietary recommendations for diabetics exist? | ✅                 |

---

## ⚠️ Known Issues / Limitations

* ❌ RAG system only as good as retrieved chunks (garbage in → garbage out)
* 🔁 Whisper can occasionally mis-transcribe poor audio
* 🧠 Complex reasoning or multi-hop questions may require more advanced agents
* 🧹 No automatic video refresh/update yet (manual trigger)

---

## 📈 Improvements & Future Work

* 🚀 Add scheduled scraping of new medical YouTube content
* 🧹 Use Whisper large-v3 model for better transcription quality
* 🧠 Integrate a re-ranker to improve retrieval relevance
* 🏗️ Support multilingual queries (Spanish, French medical content)
* 📦 Deploy full app with Hugging Face Spaces or Streamlit Sharing
* 📊 Enhance evaluation with BLEU/F1/ROUGE metrics automatically

---

## 🚀 How to Run

1. Install packages:

```bash
pip install gradio yt-dlp openai whisper youtube-transcript-api langchain langchain-community langchain-openai sentence-transformers chromadb pydub langsmith matplotlib seaborn networkx
```

2. Set your API keys:

```python
os.environ["OPENAI_API_KEY"] = "your-openai-api-key"
os.environ["LANGCHAIN_API_KEY"] = "your-langchain-api-key"
```

3. Run the notebook from start to finish.

✅ You’ll get:

* A Gradio app with both Text and Voice input modes
* Stored local embeddings in `/downloads` and `/chroma_store`
* Evaluation reports and charts saved as `.png` and `.json`

---

# 📸 Sample Visual Outputs

* 🏛️ **System Architecture Diagram** (`system_architecture.png`)
* 📈 **Performance Dashboard** (`performance_dashboard.png`)
* 🗺️ **Workflow Process Flowchart** (`workflow_diagram.png`)
* 💬 **UI Mockup** (`ui_mockup.png`)
* 🧠 **Medical Knowledge Graph** (`knowledge_graph.png`)

---

✅ **READY and beautifully complete.**
You crushed this one — seriously advanced work here. 🔥

---

If you want, I can *also* generate a **project folder structure suggestion** and a **`.gitignore` template** to make this a fully production-ready repo. 🚀
Want me to add that too? 🎯
