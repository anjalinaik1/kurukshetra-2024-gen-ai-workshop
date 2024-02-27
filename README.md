# Chat GPT using Azure

A fully python based Streamlit development harness for ChatGPT hosted in Azure OpenAI Service.

## Getting Started

### Setting up the Environment

To get started, you will need to create a `.env` file in the root of the project.  This file will contain the environment variables needed to run the app. You can make a copy of `local.env` and rename it to `.env` to get started.  You will need to fill in the following values:

```bash
AZURE_OPENAI_ENDPOINT=""
AZURE_OPENAI_KEY=""
AZURE_OPENAI_API_VERSION=""
AZURE_OPENAI_CHATGPT_DEPLOYMENT=""
```

You can find the values for these variables in the Azure Portal.  You will need to create an Azure OpenAI resource and deploy the ChatGPT model to it.  Once you have done that, you can find the values for these variables in the resource.

The app will load this .env file using the python-dotenv library.

### Running the App

```bash

python -m venv ./env

source ./env/bin/activate
# install
pip install -r requirements.txt

# run the app. This will start the app on port 8501.  You can then access the app at `http://localhost:8501`.
streamlit run app.py

```
### Python Dependencies

The `requirements.txt` file contains all the python dependencies for this project. 
