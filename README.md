# Generative AI Agents: 5-Day Course

**A collection of learning notebooks and implementations based on the Google 5-Day Gen AI Agents course.**

## 📖 About The Project

This repository serves as a practical companion to the **[Google 5-Day Gen AI Agents Course](https://www.kaggle.com/learn-guide/5-day-agents)** on Kaggle. It contains Jupyter notebooks where I deconstruct, explain, and expand upon the core concepts of building AI Agents using the Gemini API.

The goal of this project is to go beyond simple copy-pasting; each notebook includes:

* **Detailed annotations** explaining the "why" behind the code.
* **Custom experiments** to test the limits of agent reasoning.
* **Refactored implementations** using modern best practices.

This repository is also the codebase for my article series on Medium:

* *[Beyond print(): Building Production-Grade Observability in Google ADK]*
* *(More links to come)*

## 📂 Repository Structure

The project is structured to follow the curriculum of the 5-day challenge, with isolated environments managed by Poetry.

```text
.
├── notebooks/                  # Jupyter Notebooks for each module
│   ├── 01_agent_fundamentals.ipynb
│   ├── 02_prompt_engineering.ipynb
│   ├── 03_function_calling.ipynb
│   └── ...
├── .env.example                # Template for environment variables
├── pyproject.toml              # Poetry dependency configuration
├── poetry.lock                 # Locked dependency versions
├── README.md                   # Project documentation
└── .gitignore                  # Git ignore rules

```

## 🛠️ Prerequisites

Before you begin, ensure you have the following installed:

* **Python 3.10+**
* **[Poetry](https://www.google.com/search?q=https://python-poetry.org/docs/%23installation)** (Python dependency manager)
* A **[Google AI Studio API Key](https://aistudio.google.com/)**

## 🚀 Installation & Setup

This project uses Poetry to manage dependencies and a `.env` file to manage secrets securely.

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/google-genai-agents-course.git
cd google-genai-agents-course

```

### 2. Install Dependencies

Use Poetry to create a virtual environment and install all required libraries (Google Generative AI, Jupyter, etc.).

```bash
poetry install

```

### 3. Configure Environment Variables

You need to set up your API key to interact with the Gemini models.

1. Create a copy of the example environment file:
```bash
cp .env.example .env

```


2. Open the `.env` file in your text editor and add your Google API key:
```ini
GOOGLE_API_KEY=your_actual_api_key_here

```

## 💻 Usage

To run the notebooks, you need to launch Jupyter within the Poetry environment.

1. **Activate the shell:**
```bash
poetry shell

```


2. **Start Jupyter Notebook:**
```bash
jupyter notebook

```


3. Navigate to the `notebooks/` directory and open the lesson you wish to explore. The notebook handles loading the API key automatically via:
```python
from dotenv import load_dotenv
load_dotenv()

```



## 🧠 Concepts Covered

* **Prompt Engineering for Agents:** Techniques to guide Gemini's reasoning capabilities.
* **ReAct Paradigm:** Implementing Reasoning + Acting loops.
* **Tool Use (Function Calling):** Connecting Gemini to external tools and APIs.
* **Orchestration:** Managing conversation history and context windows.

## 🤝 Contributing

This is a personal learning repository, but suggestions and discussions are welcome! If you find a bug or have a suggestion for a better implementation, feel free to open an issue.

## 📜 License

Distributed under the Apache-2.0 License. See `LICENSE` for more information.

## 🔗 Acknowledgements

* [Google AI Studio](https://aistudio.google.com/)
* [Kaggle Learn](https://www.kaggle.com/learn)
* The open-source community for the tools used in this repo.
