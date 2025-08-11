MCQ Generation using LangChain

Generates Multiple Choice Questions (MCQs) from text using LangChain, Google GenAI API, and Pydantic.

   Requirements
- Python 3.9+
- Packages:
  - `langchain` → `pip install langchain`
  - `google_genai_api` → `pip install langchain-google-genai`
  - `pydantic` → `pip install pydantic`
  - `python-dotenv` → `pip install python-dotenv`

   Setup
1. Put `MCQ_Generation.ipynb` in the project root.
2. (Optional) Create `requirements.txt` with:
    ```
    langchain
    googleGenAI
    pydantic
    python-dotenv
    ```
3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Add your GoogleGenAI API key in a `.env` file:
    ```
    GOOGLE_API_KEY=your_api_key_here
    ```

   Usage
1. Open the notebook:
    ```bash
    jupyter notebook MCQ_Generation.ipynb
    ```
2. Provide input text in the notebook and run cells to generate MCQs.

   Example output
```json
{
  "questions": [
    {
      "question": "Who developed the theory of relativity?",
      "options": ["Isaac Newton", "Albert Einstein", "Galileo Galilei", "Nikola Tesla"],
      "answer": "Albert Einstein"
    }
  ]
}
