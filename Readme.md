# Project README

**AI Legal Reasoning Assistant (DeepSeek R1 & RAG)** 

Designed a legal analysis tool using DeepSeek R1 to leverage Chain-of-Thought (CoT) reasoning for interpreting complex legal statutes. Built a RAG pipeline with LangChain and FAISS to retrieve context from penal codes (e.g., UDHR), reducing hallucinations and providing citation-backed legal answers via a Streamlit interface.
---

## Table of Contents
1. [Environment Setup](#environment-setup)
    - [Using Conda](#using-conda)
    - [Using Pip](#using-pip)
2. [Running the Project](#running-the-project)

---

## Environment Setup


### Using Conda
Conda is an open-source package management system and environment management system.

1. Create a new conda environment:
    ```
    conda create -n myenv python=3.9
    ```

2. Activate the environment:
    ```
    conda activate myenv
    ```

3. Install dependencies from `requirements.txt` (if available):
    ```
    pip install -r requirements.txt
    ```

---

### Using Pip
Pip is the standard package installer for Python.

1. Install virtualenv if you don't have it:
    ```
    pip install virtualenv
    ```

2. Create a virtual environment:
    ```
    virtualenv venv
    ```

3. Activate the virtual environment:
    - On Windows:
        ```
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```
        source venv/bin/activate
        ```

4. Install dependencies from `requirements.txt` (if available):
    ```
    pip install -r requirements.txt
    ```

---

## Running the Project

The project consists of three Python files, each corresponding to a different phase of the project:

### To run the App directly
```
streamlit run main.py
```

### To run app in different phases

1. Phase 1: Run the first phase using:
    ```
    streamlit run frontend.py
    ```

2. Phase 2: Run the second phase using:
    ```
    python vector_database.py
    ```

3. Phase 3: Run the third phase using:
    ```
    python rag_pipeline.py
    ```



---
