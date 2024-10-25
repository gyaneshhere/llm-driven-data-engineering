# LLM-driven Data Engineering

## Getting Started

Make an OpenAI account [here](https://platform.openai.com/) and then generate an API Key.

## Setup

Store the API key as an environment variable like:
`export OPENAI_API_KEY=<your_api_key>`
Or set it in Windows

The easiest way to install the dependencies is uv. [Install](https://docs.astral.sh/uv/getting-started/installation/) it.

Run the command `uv sync` to install the python environment and all of the libraries under `.venv` folder.

You should configure your IDE to select the interpreter under the .venv folder, or activate it through the command on your terminal:
```sh
source .venv/bin/activate
```

PS: If you don't want to use uv, run
```sh
pip install .
```


 - `pg_restore -h localhost -p 5432  -d postgres -U <your laptop username> halo_data_dump.dump`

Add it to the environment `export PINECONE_API_KEY=<your pinecone API key>`


