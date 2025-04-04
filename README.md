# **Getting Started with Mistral**

## **Course Overview**

[**Getting Started with Mistral**](https://www.deeplearning.ai/short-courses/getting-started-with-mistral/) introduces learners to Mistral AI’s open-source and commercial large language models (LLMs), including Mistral 7B, Mixtral 8x7B, and Mixtral 8x22B. The course guides you through selecting the right model for your use case, making API calls, and implementing advanced features such as JSON mode, function calling, and Retrieval-Augmented Generation (RAG). You’ll also build a chat interface for document-based Q&A systems.

By the end of this course, you'll be able to:
- Choose and integrate Mistral models via API.
- Use prompting techniques for structured and advanced tasks.
- Implement function calling to interact with external tools.
- Build a basic RAG system using vector search.
- Create a chat UI to interact with models and uploaded documents.


## **Course Content**

1. [**Introduction to Mistral Models**]
   - Overview of Mistral’s model lineup and their capabilities.
   - Model selection based on complexity, performance, and cost.

2. [**Prompting Capabilities**]()
   - Prompt engineering techniques for classification, summarization, personalization, grammar correction, and JSON extraction.
   - API integration for structured responses.

3. [**Model Selection**]()
   - Practical guidance on when to use Mistral Small, Medium, and Large models.
   - Use case demonstrations: spam filtering, email generation, expense reporting, and code generation.

4. [**Function Calling**]()
   - Automating tool selection and external function invocation through Mistral’s function calling framework.
   - Sample application: querying a transaction dataset.

5. [**Retrieval-Augmented Generation (RAG)**]()
   - Building a RAG pipeline with FAISS, web scraping, and Mistral embeddings.
   - Enhancing responses using contextual document retrieval.

6. [**Chat Interface & RAG UI**]()
   - Developing a user interface with the Panel library.
   - Switching between standard chat and RAG-based Q&A with document upload support.


## **Notebooks**

The following Jupyter notebooks are included to support hands-on learning:

- [L2_prompting_capabilities.ipynb]() – Explore prompt engineering and JSON mode with Mistral models.
- [L3_model_selection.ipynb]() – Learn how to select and apply different Mistral models for specific tasks.
- [L4_function_calling.ipynb]() – Implement and integrate function calling with tool selection and execution.
- [L5_basic_RAG.ipynb]() – Build a basic RAG system using Mistral embeddings and FAISS.
- [L6_chat_ui.ipynb]() – Create a user-friendly chat interface with document RAG capabilities.
- [AI_greenhouse_gas.txt]() – (Text file, content-specific example)
- [helper.py]() – Helper functions for loading API keys and managing calls.
- [requirements.txt]() – Required Python dependencies.


## **Getting Started**

1. **Install Dependencies**
   Ensure Python 3.8+ is installed. Then install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

2. **Set Up API Key**
   Store your Mistral API key in a `.env` file:
   ```
   MISTRAL_API_KEY=your_api_key_here
   ```
   Load it using the helper script:
   ```python
   from helper import load_mistral_api_key
   load_mistral_api_key()
   ```

3. **Run Notebooks**
   Open the notebooks in Jupyter or VSCode and follow the step-by-step cells to explore each concept.


## **Resources and References**

- [Mistral AI Chat](https://chat.mistral.ai/chat)
- [Mistral AI Docs](https://docs.mistral.ai)
- [Advanced Retrieval for AI (Chroma)](https://learn.deeplearning.ai/courses/advanced-retrieval-for-ai/lesson/1/introduction)
- [Building and Evaluating Advanced RAG](https://learn.deeplearning.ai/courses/building-evaluating-advanced-rag)


## **Helpers & Utils**

- **helper.py**
  - `load_mistral_api_key()` – Loads your API key from `.env` using `python-dotenv`.
  - Utility functions simplify authentication and setup across notebooks.

