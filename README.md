Here is a professionally formatted README.md file based on your content. I have organized it to follow standard GitHub documentation best practices, ensuring clarity, readability, and proper rendering of the diagrams.You can copy the code block below directly into your repository.Markdown# 🎯 NLP2SQL

<div align="center">

> **Transform natural language into powerful SQL queries with ease!**

[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit)](https://streamlit.io/)
[![Azure OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=flat-square&logo=microsoft)](https://azure.microsoft.com/en-us/products/ai-services/openai-service)
[![Gemini](https://img.shields.io/badge/Gemini-FF6F61?style=flat-square&logo=google)](https://deepmind.google/technologies/gemini/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql)](https://www.postgresql.org/)
[![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite)](https://www.sqlite.org/index.html)

</div>

---

## 📖 Overview

**NLP2SQL** is an advanced tool designed to bridge the gap between natural language and database management. By leveraging the power of **Azure OpenAI** and **Google Gemini**, this application allows users to interact with their databases using plain English. Whether you need to generate complex SQL queries, visualize data trends, or analyze statistics, NLP2SQL handles the heavy lifting securely and efficiently.

## ✨ Features

### 🎯 Core Capabilities
- **Natural Language to SQL** 🗣️ → 📝
  - Convert text queries into SQL commands automatically.
  - Intelligent query interpretation with detailed decision logs and step-by-step reasoning.
- **Multimodal Interaction** 🎥
  - Process both textual and visual inputs for richer query context.
- **Multi-Database Support** 🗄️
  - **SQLite:** Easy file upload and compatibility.
  - **PostgreSQL:** Secure integration with remote databases.
  - Dynamic schema exploration.

### 📊 Visualization & Analytics
- **Dynamic Visualizations** 📈
  - AI-powered recommendations for the best chart type.
  - Supported charts: Bar, Line, Scatter, Area, and Histogram.
- **Interactive Data Explorer** 🔍
  - Real-time data filtering, sorting, and exploration.
- **Summary Statistics** 📋
  - Detailed numeric analysis (mean, median, mode, skewness, kurtosis).
  - Categorical data insights and distribution analysis.

### 🛡️ Security & Management
- **Safe SQL Execution** 🔒
  - Strict query validation and SQL injection prevention.
  - Comprehensive error handling.
- **Query History** 📚
  - Searchable query logs with export options (CSV, Excel, JSON).

---

## 🏗️ Architecture

```mermaid
graph LR
    A[User Input] --> B[LLM Processing]
    B --> C[SQL Generator]
    C --> D[Database]
    D --> E[Results]
    E --> F[Visualization]
🚀 Getting StartedFollow these steps to set up the project locally.1️⃣ Clone the RepositoryBashgit clone [https://github.com/lohitkolluri/NLP2SQLL.git](https://github.com/lohitkolluri/NLP2SQLL.git)
cd NLP2SQL
2️⃣ Set Up Environment VariablesCreate a .env file in the root directory and configure your API keys. You can choose between Azure OpenAI or Gemini (or configure both).Content for .env:Ini, TOML# --- Option 1: Azure Configuration ---
LLM_PROVIDER=AZURE
OPENAI_ENDPOINT="https://[ENDPOINT_NAME].openai.azure.com"
OPENAI_API_VERSION="2024-08-01-preview"
OPENAI_API_KEY="YOUR_AZURE_OPENAI_API_KEY"
MODEL_NAME="YOUR_AZURE_DEPLOYMENT_NAME"

# --- Option 2: Gemini Configuration ---
# LLM_PROVIDER=GEMINI
GEMINI_API_KEY="YOUR_GEMINI_API_KEY"
3️⃣ Install DependenciesBashpip install -r requirements.txt
4️⃣ Launch the AppBashstreamlit run app/NLP2SQL.py
💡 How It WorksQuery Input: Enter a question in plain English (e.g., "Show me the top 5 sales by region").Processing: The LLM (Azure OpenAI or Gemini) analyzes the schema and generates the appropriate SQL.Validation: The system validates the query for safety and correctness.Execution: The query runs against your selected database (PostgreSQL or SQLite).Analysis: Results are processed to generate summary statistics.Visualization: The data is presented with AI-recommended interactive charts (Plotly).Export: Download your results in CSV, Excel, or JSON formats.🛠️ Built WithTechnologyPurposeStreamlitInteractive Web InterfaceAzure OpenAINLP & Logic ProcessingGeminiNLP & Logic ProcessingPostgreSQLEnterprise Database SupportSQLiteLightweight Database SupportPlotlyInteractive Visualizations🌟 Feature MapCode snippetmindmap
  root((NLP2SQL))
    Query Processing
      Natural Language Input
      Decision Logging
      Detailed Reasoning
    Visualization
      Interactive Charts
      Summary Statistics
      Data Distribution
    Database
      PostgreSQL
      SQLite
      Schema Analysis
    Security
      Query Validation
      Error Handling
      Safe Execution
