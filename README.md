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

## Day 1 Lab

We'll be using the schemas from Dimensional Data Modeling Week 1 and generating the queries from the homework and labs except this time we'll do it via LLMs

## Day 2 Lab

We'll be using Langchain to auto generate SQL queries for us based on tables and writing LinkedIn posts in Zach Wilson's voice
### Setup

If you are watching live, you will be given a cloud database URL to use.
`export LANGCHAIN_DATABASE_URL=<value zach gives in Zoom>`

If you aren't watching live, you'll need to use the `halo_data_dump.dump` file located in the `data` folder

Running `pg_restore` with your local database should get you up and running pretty quickly. 

- example command, assuming you got Postgres up and running either via Homebrew or Docker:
 - `pg_restore -h localhost -p 5432  -d postgres -U <your laptop username> halo_data_dump.dump`

## Day 3 Lab

This lab leverages this [repo](https://github.com/DataExpert-io/auto-feedback-example)

## Day 4 Lab
This lab leverages this [repo](https://github.com/DataExpert-io/vector-database-example)

Add it to the environment `export PINECONE_API_KEY=<your pinecone API key>`


