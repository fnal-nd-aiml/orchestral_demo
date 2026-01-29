# Orchestral-AI Demo

This repo contains some notebooks to show some applications of [Orchestral AI](https://orchestral-ai.com) for AI Operations at Fermilab.

## Orchestral Installation

Tested on MacOS.
Instructions to run on GPVM will come soon.

```bash
# Oschestral works with Python 3.13
pyenv install 3.13.0

# Set python 3.13 in your local directory only
pyenv local 3.13.0

# Create a virtual environment
python -m venv .venv-py313

# If you don't have pyenv, you can install it with
# curl https://pyenv.run | bash

# Activate the environment
source .venv-py313/bin/activate

# Install needed software
pip install jupyterlab ipykernel
python -m ipykernel install --user --name py313 --display-name "Python 3.13"
pip install google-api-core

# Install orchestral
pip install orchestral-ai
```

Orchestral needs the API key if you decide to use some cloud models
```bash
OPENAI_API_KEY=sk-...           # For GPT models
ANTHROPIC_API_KEY=sk-ant-...    # For Claude models
GOOGLE_API_KEY=...              # For Gemini models
GROQ_API_KEY=gsk_...            # For Groq (fast inference)
MISTRAL_API_KEY=...             # For Mistral models
```
You can add these in a `.env` file in your project directory. Otherwise, download Ollama and use a local model (see below).

## ECL-API Installation

Install the ecl-api package:
```bash
pip install ecl-api
```
This package allows interacting with the e-log from Python. More info: https://github.com/marcodeltutto/ecl-api.


## Ollama Installation

Go to [Ollama](https://ollama.com) and download Ollama on your Mac. Open the application and select `gpt-oss:20b`, click on the download symbol next to it. This will download the Open AI `gpt-oss:20b` on your computer. 
