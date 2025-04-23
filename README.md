![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Project | Business Case: Building a Multimodal AI ChatBot for YouTube Video QA (or similar)

## Instructions

The goal of this project is to leverage state-of-the-art techniques and technologies, including **LangChain**, to develop an innovative AI **multimodal question-answering** application with real-world impact. You can choose between two options:

- **Ironhack Project Template**
- **Your Own Project Idea** (must meet certain requirements – see section "Requirements")

This final project offers an exciting opportunity to explore the intersection of **NLP**, **speech recognition**, and **multimedia analysis**. You may wish to focus your application on a particular domain like health, nutrition, astrophysics, or real-time translation... As such, feel free to build something you will be proud of. Read carefully the instructions for each project option below, before reviewing the project requirements and evaluation criteria.

### Ironhack Project Template vs Your Own Project Idea

| **Ironhack Project Template** | **Your Own Project Idea** |
|------------------------------|----------------------------|
| **Objective**: Build a chatbot that can translate YouTube videos into text and allow natural language querying. | **Objective**: Create a bespoke application that solves a **multimodal question/answering** task. |
| **Use Cases**:<br>• Improve **accessibility** for users with hearing impairments or those who prefer reading over watching videos, thereby broadening the audience reach and enhancing brand reputation.<br>• Enable **efficient indexing and searching** of video content, allowing users to quickly find specific information within videos, which is particularly useful for educational content and tutorials.<br>• Improve **customer support** by leveraging existing video content to provide instant, accurate responses to customer queries, thus reducing support costs and improving response times.<br>• Improve **SEO and multilingual engagement** <br> • Serve **educational and training purposes** by enhancing the learning experience, enabling easy querying and access to specific segments of instructional videos. | **Examples**:<br>• Answer questions in **audio** instead of text<br>• Build agent to answer questions about a **database of images**<br>• Build a **real-time speech translator** with subtitles |
| **Project Overview**:<br>Develop a RAG system or AI bot that combines the power of text and audio processing to answer questions about YouTube videos. The bot will utilize natural language processing (NLP) techniques and speech recognition to analyze both textual and audio input, extract relevant information from YouTube videos, and provide accurate answers to user queries. Some useful resources include [Whisper](https://huggingface.co/openai/whisper-large-v3) from OpenAI. | **Requirements**:<br>Your idea must meet the same **project requirements** as the template option. We recommend setting a goal and starting off with an MVP that meets these requirements before expanding. <br> If you choose this, you must **notify the teaching team by Day 2 (28th April)**. |
| **Key Objectives**:<br>• Develop a text-based QA model with pre-trained language models<br>• Integrate speech recognition capabilities to convert audio/video input (user questions) into text transcripts. Beware that there is a [YouTube](https://pypi.org/project/youtube-transcript-api/) Python module that retrieves pre-existing subtitles, often auto-generated and error-prone. That’s why you should use a speech-to-text AI  for transcription.<br>• Build a conversational interface for users to interact with the bot via text or voice input. The latter is not a must. <br>• Retrieve, analyse, and store into a vector database (pinecone, chromabd...) YouTube video content to generate answers to user questions. <br>• Test and evaluate the bot's performance in accurately answering questions about YouTube videos. <br>• YouTube Video Retrieval: Develop LangChain agents for accessing YouTube video content and extracting relevant metadata for analysis. | **Project Suggestion Tips**:<br>• Start with an MVP<br>• Ensure multimodal processing<br>• Clearly define architecture and data used<br>• Think accessibility, creativity, real-world utility |

## Resources

- Pre-trained language models available in libraries like [HuggingFace](https://huggingface.co/) Transformers.
- [LangChain](https://python.langchain.com/v0.1/docs/get_started/quickstart/) for text preprocessing, model development, and conversational interface design.
- [LangSmith](https://www.langchain.com/langsmith) for testing, performance checks, and [deploying](https://langchain-ai.github.io/langgraph/cloud/quick_start/#test-the-graph-build-locally) your model and app.

## Evaluation Criteria

- Building of an AI pipeline that can perform a multimodal question-answering task.
- Testing of the AI on metrics like accuracy, hallucination, context relevancy, etc. 
- Writing of clean, modular, and efficient code following best practices.
- Documentation of the AI app features, configurations, and technical specifications.
- Delivery of a presentation and performance of a demo to deliver your final results to the class.
- Saving and tracking changes in the source code using Git and GitHub.
- Ensuring the AI is deployed and optimized for latency.

## Requirements (these apply to both project options)

### 1. Code

- **Multimodal Pipeline** (for example: text-to-speech, vision-to-speech, speech-to-text. This means that text-to-text would not be appropriate).
- Use **LangChain** agents and functions for:
  - Text preprocessing (e.g., tokenize)
  - QA model development: use OpenAI API or HuggingFace
  - Speech recognition integration: integrate speech recognition capabilities into the bot, allowing it to process audio and/or text inputs
  - Conversational interface: use LangChain agents to handle user interactions and route queries to the appropriate processing modules.
  - Using a vector database of your choice
  - Using LangSmith platform for testing, evaluation, and deployment
- Agentic AI (several tools and models)
- Local and/or Cloud Deployment
- In-depth Documentation

### 2. Data

**Data must NOT be sourced in Saudi Arabia** due to legal restrictions.

### 3. Presentation

- Duration: **15–20 minutes**
- Do not include minute details (for example, learning rate values or hyperparameter tuning. However, you could be asked about these by the teachers).
- Include the logic behind your architecture design decisions. This means that we need to know that your choices were made scientifically and not randomly.
- Your performance slides must include the baseline performance as a reference for subsequent improvements and decision-making.
- Evaluation slides should include how you dealt with common issues such as hallucinations and relevancy. They must also address the context of latency, cost, memory requirements, and future proofing.
- Do NOT include too much text. We also recommend light color backgrounds.

## Timeline

| Day | Tasks |
|-----|-------|
| 1–2 | - Project selection <br> - Data collection <br> - Deadline for informing the teaching team of project selection. This includes: <br> 1. Explaining if Option 1 or 2 is chosen. <br> 2. Which data is to be used. <br> 3. A clear high-level overview of the deployed product. |
| 3   | Model development |
| 4–6 | Interface development |
| 7–8 | - Testing <br> - Evaluation <br> - Documentation <br> - Deployment <br> - Presentation preparation |

## Deliverables

The final deliverable should be a **GitHub repository** containing the following:

1. **Source Code**
   - Code implementation of the multimodal AI bot
   - Code of experiments (even for things that don’t make it in production!)
   - Code for deployment (inside a `/deployment` folder)
   - Clean, modular and efficient code following best practices
2. **README.md**
   - Clear explanation of the project goal and architecture
   - Methodology used for building and testing the system
   - Setup instructions, repository structure, configurations (`requirements.txt` file) and usage guide
3. **Presentation Slides**