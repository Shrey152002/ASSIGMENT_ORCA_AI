## Installation Guide

1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```


---

## Usage Instructions

1. Run the application:
    ```bash
    python app.py
    ```

2. Open the application in your browser (default URL: `http://127.0.0.1:7860`).

3. Input the following:
    - **Context:** A passage of text for the models to analyze.
    - **Questions:** A list of questions (one per line).
    - **Ground Truth:** The expected answers (one "Yes" or "No" per line).

4. View the comparison results, including:
    - Responses from both models.
    - Accuracy of each model.

---

## Models Used

1. **Groq's `llama3-70b-8192`**: This model is accessed via the Groq API and is used for extracting boolean information from text. It is designed for high precision and is optimized for boolean question-answering tasks.

2. **OpenAI's `gpt-4-turbo`**: This model is accessed via the OpenAI API. It is a versatile, state-of-the-art language model capable of answering boolean questions based on the provided context and questions.

Both models are queried with the same set of questions and context to evaluate their accuracy against the provided ground truth answers.
