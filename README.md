# RAG Chatbot with Mistral AI - Personal RAG Testing Toolkit

A Retrieval-Augmented Generation (RAG) chatbot built with Flask and Mistral AI. Use this repository to experiment with your own RAG-based implementations and see how the retrieval process impacts generated answers.

Originally created by Michael Bushnell, the project has been adapted so you can quickly run tests with your own documents. Swap out the example text, tweak the prompt logic in `mistral_rag.py`, or connect a different vector store to explore new approaches.

## Setup

1. Clone the repository.
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with your Mistral API key:
   ```
   MISTRAL_API_KEY=your_api_key_here
   ```
5. Add any text you want to test as `essay.txt` in the project root.

## Local Development

Run the Flask application:

```bash
python app.py
```

The app will be available at `http://localhost:5001`. Interact with the chatbot to observe how the RAG pipeline responds to your content.

## Deployment to Vercel

1. Push your code to GitHub.
2. Connect the repository to Vercel.
3. Add your environment variables in the Vercel dashboard:
   - `MISTRAL_API_KEY`: your Mistral API key
4. Deploy and share your RAG demo.

## Environment Variables

- `MISTRAL_API_KEY`: Mistral AI API key (required)

## Project Structure

- `app.py`: Flask application entry point
- `mistral_rag.py`: Helper functions for the RAG workflow
- `templates/`: HTML templates
- `static/`: Static files (CSS and JavaScript)
- `essay.txt`: Source text for your experiments
- `requirements.txt`: Python dependencies
- `vercel.json`: Vercel deployment configuration

## Usage and Licensing

This repository is intended for your personal exploration of RAG techniques. Use it as a starting point to prototype ideas, run workshops, or incorporate RAG into your own projects.

Feel free to reach out to [Halim Madi](https://www.halimmadi.com) with any questions or feedback!

