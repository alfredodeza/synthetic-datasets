# Create Synthetic Data using Large Language Models

Augment datasets using Large Language Models by generating synthetic data. This repository has simple examples you can use to generate Synthetic Data and persist it to disk as a CSV file.

## Setup your environment

This example can run in Codespaces but you can use the following if you are
cloniing this repository:

**Install the dependencies**

Create the virtual environment and install the dependencies:

```
python3 -m venv .venv
source .venv/bin/activate
.venv/bin/pip install -r requirements.txt
```

Here is a summary of what this repository will use:

1. [Llamafile](https://github.com/Mozilla-Ocho/llamafile) for the LLM (alternatively you can use an OpenAI API compatible key and endpoint)
1. [OpenAI's Python API](https://pypi.org/project/openai/) to connect to the LLM after retrieving the vectors response from Qdrant
1. A large language model (LLM) to generate synthetic data like [Mixtral](https://huggingface.co/jartine/Mixtral-8x7B-Instruct-v0.1-llamafile/resolve/main/mixtral-8x7b-instruct-v0.1.Q5_K_M.llamafile?download=true) or using an OpenAI API based service. 

## Lessons

1. [Connect to an OpenAI based service](./examples/1-openai-api/example.ipynb)
1. [Generate Synthetic Data](./examples/2-generate-data/example.ipynb)
1. [Persist and verify the Synthetic Data](./examples/3-persist-and-verify/example.ipynb)