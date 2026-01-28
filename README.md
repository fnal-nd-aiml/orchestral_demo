# Orchestral-AI Demo

## Installation

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

Install the ecl-api package:
```bash
pip install ecl-api
```
This package allows interacting with the e-log from Python. More info: https://github.com/marcodeltutto/ecl-api.
