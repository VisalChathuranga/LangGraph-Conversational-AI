# LangGraph Conversational AI Agent: A Journey Through Stages 1–4

Welcome to the **LangGraph Conversational AI Agent** repository! 🚀 Dive into this exciting collection of Jupyter notebooks (`LangGraph_stage_1.ipynb` to `LangGraph_stage_4.ipynb`), where you’ll explore the development of a cutting-edge conversational AI system using **LangGraph**—a powerful library from LangChain for crafting stateful, multi-agent workflows. Whether you’re a developer, AI enthusiast, or researcher, this hands-on guide unlocks the secrets of building intelligent, tool-augmented agents with ease!

## 🌍 What is This Repository About?

This repository takes you on a thrilling step-by-step journey to create a conversational AI agent powered by **LangGraph**. Starting with the basics in Stage 1, each notebook builds momentum, culminating in a state-of-the-art agent in Stage 4 that harnesses tools like document retrieval and web search for smart query responses. The core strength lies in LangGraph’s graph-based architecture, seamlessly managing complex workflows, preserving conversation state, and orchestrating interactions between language models, tools, and users.

Packed with clear code examples, detailed explanations, and stunning visualizations, these notebooks are both educational and practical. By the end, you’ll master the art of crafting scalable, modular AI systems with LangGraph!

## 💡 Key Features

- **Progressive Learning Path**: Four stages evolve from LangGraph basics to advanced agentic workflows, perfect for beginners and experts alike.
- **Stateful Conversations**: Master maintaining conversation state with `StateGraph` and `AgentState` for context-aware agents.
- **Tool Integration**: Discover how to connect tools (e.g., document retriever, DuckDuckGo search) to a language model for enhanced capabilities (Stage 4).
- **Graph Visualization**: Admire agent workflows with Mermaid diagrams crafted from LangGraph’s structure (Stage 4).
- **Real-World Application**: Witness LangGraph in action with a dynamic conversational AI that fetches relevant info on the fly.
- **Modular Code**: Enjoy well-documented Jupyter notebooks with reusable code for easy experimentation.

## 📚 Stage-by-Stage Breakdown

### Stage 1: Foundations of LangGraph
- **Objective**: Kick off with LangGraph’s core concepts—`StateGraph`, nodes, and edges.
- **Highlights**:
  - Set up a simple LangGraph workflow with a single node and edge.
  - Define a basic state to track messages.
  - Launch a minimal conversational loop with a language model.
- **Why It Matters**: Establishes the foundation for LangGraph’s graph-based agent design.
- ![Stage 1](Images/1.png)

### Stage 2: Building a Simple Conversational Agent
- **Objective**: Craft a basic conversational AI agent that processes queries and retains state.
- **Highlights**:
  - Build a multi-node graph with a language model node and response handler.
  - Utilize `HumanMessage` and `SystemMessage` for smooth conversation flow.
  - Add conditional edges for dynamic routing based on user input.
- **Why It Matters**: Showcases LangGraph’s ability to enable context-aware chats with simplicity.
-  ![Stage 2](Images/2.png)

### Stage 3: Enhancing with Tools and Conditional Logic
- **Objective**: Boost the agent with external tools and smart routing logic.
- **Highlights**:
  - Integrate a tool (e.g., mock retriever or calculator) with the language model.
  - Implement `should_continue` logic to decide tool invocation or conversation end.
  - Expand the state to manage tool calls and responses.
- **Why It Matters**: Demonstrates LangGraph’s support for tool-augmented, dynamic agents.
- ![Stage 3](Images/3.png)

### Stage 4: Advanced Stateful Agent with Tool Integration
- **Objective**: Develop a fully functional, stateful AI agent with real-world tools.
- **Highlights**:
  - Integrate Google Gemini (`ChatGoogleGenerativeAI`) for powerful query processing.
  - Leverage a Chroma vector store for PDF-based document retrieval.
  - Add DuckDuckGo search for real-time web queries.
  - Design a complex `StateGraph` with nodes for `call_llm` and `take_action`.
  - Visualize workflows with a Mermaid diagram.
  - Manage tool calls with `ToolMessage` and conversation history with `AgentState`.
- **Why It Matters**: Unites all concepts into a production-ready agent, highlighting LangGraph’s real-world potential.
- ![Stage 4](Images/4.png)

## 🛠️ Technologies Used

- **LangGraph**: Powers stateful, graph-based agent workflows.
- **LangChain**: Drives language model integration (`ChatGoogleGenerativeAI`), embeddings (`GoogleGenerativeAIEmbeddings`), and tools (`DuckDuckGoSearchRun`).
- **Chroma**: Enables efficient vector-based document retrieval.
- **PyPDF**: Handles PDF loading and processing.
- **Python**: Core language with libraries like `google-generativeai`, `langchain_chroma`, and `langchain_community`.
- **Jupyter Notebooks**: Offers an interactive space for code, explanations, and visualizations.

## 💻 Getting Started

### Prerequisites
- **Python 3.8+**
- **Jupyter Notebook or JupyterLab**
- **Google Gemini API Key**: Set as `GEMINI_API_KEY` in your environment or via `google.colab.userdata`.
- **Required Packages**: Install via `requirements.txt` or notebook pip commands (details in notebooks).

### Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/VisalChathuranga/LangGraph-Conversational-AI.git
   cd LangGraph-Conversational-AI
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure your API key:
   - In Colab: Use `userdata.get('GEMINI_API_KEY')`.
   - Locally: `export GEMINI_API_KEY=your-api-key`.

### Running the Notebooks
1. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
2. Start with `LangGraph_stage_1.ipynb` and progress through the stages.
3. For Stage 4, add a PDF document in the working directory for the retriever.
4. Run cells to experience the agent’s evolution from basics to advanced tools.

## 🎯 Use Cases
- **AI Development**: Build stateful, tool-augmented agents for chatbots, virtual assistants, or Q&A systems.
- **Research**: Test LangGraph’s graph architecture for multi-agent or complex workflows.
- **Education**: Use as a teaching tool for AI, NLP, or agentic system courses.
- **Industry Prototyping**: Prototype agents for document-based QA or automated support.

## 🙌 Acknowledgments
- **LangChain**: For the innovative LangGraph library and ecosystem.
- **Google Gemini**: For powering the language model.
- **Chroma**: For top-notch vector storage and retrieval.
- **Community**: Gratitude to the open-source community for inspiration and tools.

---

*🌈 Ready to embark on your LangGraph adventure? Clone this repo and explore the notebooks now—let’s build intelligent agents together!*
