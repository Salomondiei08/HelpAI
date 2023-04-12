# HelpAI

![HelpAI Logo](assets/banner.gif)

HelpAI is an open-source Python project that utilizes OpenAI GPT3/GPT4 models alongside Longchin to create a customer service AI agent to answer customer questions. The project works by vectorizing and storing all the data provided on the help center website of the company in a Pinecone database. It then vectorizes the query entered by the user and performs a similarity check to retrieve essential data and pass it in the command sent to GPT4. 

## How to Set Up HelpAI

To set up HelpAI, follow these steps:

1. Create a Python environment by running `python -m venv <env-name>`
2. Install all dependencies by running `pip install -r requirements.txt`
3. Create an account on the [OpenAI](https://openai.com/) and get an API Key
4. Create an account on [Pinecone](https://www.pinecone.io/) and create an index called `help-ai` with a dimension of 1536
5. Create the `utils/secret_keys.py` file, create and fill the `OPENAI_API_KEY`, `PINECONE_API_KEY`, and `PINECONE_ENVIRONMENT` constants with your OpenAI API Key, Pinecone API Key, and Pinecone environment

## How to Run HelpAI

To run HelpAI:

1. Vectorize and store the data in your Pinecone index by running `python create_index.py`
2. Run and query the program by running `python main.py`

## Contributing to HelpAI

We welcome contributions from anyone interested in improving HelpAI! To contribute:

1. Fork the repository and clone it to your local machine
2. Create a new branch for your feature or bug fix
3. Make your changes and commit them to your branch
4. Push your changes to your forked repository
5. Create a pull request to merge your changes into the main branch

Thank you for your interest in contributing to HelpAI!

## Contributors

- DIEI Salomon
- ADJETEY Michel
