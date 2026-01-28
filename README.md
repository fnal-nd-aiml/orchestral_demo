# Orchestral-AI Demo

## Orchestral Installation

Tested on MacOS.
Instructions to run GPVM will come soon.

```bash
pyenv install 3.13.0
pyenv local 3.13.0
python -m venv .venv-py313
source .venv-py313/bin/activate
pip install jupyterlab ipykernel
python -m ipykernel install --user --name py313 --display-name "Python 3.13"
pip install orchestral-ai
pip install google-api-core
```

## ECL-API Installation

Install the ecl-api package:
```bash
pip install ecl-api
```
This package allows interacting with the e-log from Python. More info: https://github.com/marcodeltutto/ecl-api.


## Ollama Installation

Go to https://ollama.com and download Ollama on your Mac. Open the application and select `gpt-oss:20b`, click on the download symbol next to it. This will download the Open AI `gpt-oss:20b` on your computer. 
