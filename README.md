# Deckpilot AI

Deckpilot AI is a lightweight assistant designed to run locally while leveraging OpenAI's APIs for language tasks. The project contains a minimal wrapper around the OpenAI client so you can easily integrate generative AI features into your own tools.

## Setup Requirements

- **Python 3.10 or newer**
- Required packages: `openai` and optionally `python-dotenv` if you wish to load API keys from a `.env` file.

Install the packages with:

```bash
pip install openai python-dotenv
```

You also need an OpenAI API key set in the `OPENAI_API_KEY` environment variable.

## Example Usage

Below is a simple example that calls the OpenAI wrapper to generate a completion.

```python
from deckpilot.openai_wrapper import ask

response = ask("Hello, Deckpilot!")
print(response)
```

The `ask` function forwards your prompt to the OpenAI API and returns the assistant's reply.
