# Sequential-workflow-Langgraph

This repository contains example workflows built with `langgraph` and notebook-driven state graphs.

## Notebooks

- `prompt_chain_workflow.ipynb`
  - Builds a sequential prompt chain for blog generation.
  - Uses a `StateGraph` with two nodes: `create_outline` and `create_blog`.
  - Demonstrates compiling the workflow, visualizing the graph, and invoking the workflow with an initial title.

- `qa_llm_workflow.ipynb`
  - Builds a simple question-answer workflow using a `StateGraph`.
  - Uses one node: `llm_qa`.
  - Demonstrates compiling the workflow and invoking it with a question.

## Requirements

- Python 3.11+ (or compatible)
- `langgraph`
- `langchain_google_genai`
- `python-dotenv`
- `ipython` / Jupyter Notebook

## Usage

1. Install requirements.
2. Create a `.env` file with any required API keys.
3. Open the notebooks in Jupyter or VS Code.
4. Run cells in order to build and execute the workflows.

## Notes

- The notebooks assume a Google Gemini-compatible LLM integration.
- Update the model, temperature, and environment variables as needed.
