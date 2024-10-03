
# OpenAI ChatGPT with Python

This repository demonstrates how to connect Python to OpenAI's ChatGPT API using the `openai` Python package. It allows you to send prompts to ChatGPT and receive responses directly from a Python script.

## Features

- **Interactive Prompts:** Users can input any question or prompt, and the script will return a response from ChatGPT.
- **OpenAI API Integration:** Utilizes the official OpenAI API for seamless interaction.
- **Customizable Parameters:** Easily adjust the model, response length, and creativity of responses through code parameters.

## Requirements

Before you start, ensure you have the following:

- Python 3.6+
- OpenAI API Key (You can sign up for an API key [here](https://platform.openai.com/signup))

## Installation

### Step 1: Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/your-username/openai-chatgpt-python.git
cd openai-chatgpt-python
```

### Step 2: Install the Required Dependencies

Install the dependencies listed in the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### Step 3: Set Up Your OpenAI API Key

You'll need to provide your OpenAI API key to authenticate requests. You can do this in two ways:

1. **Set the API key as an environment variable** (recommended for security):

    ```bash
    export OPENAI_API_KEY="your-api-key"
    ```

2. **Hardcode the API key in the script**: Replace `'your-api-key'` in `chatgpt.py` with your actual API key:

    ```python
    openai.api_key = 'your-api-key'
    ```

## Usage

Once everything is set up, run the Python script and enter your prompt:

```bash
python chatgpt.py
```

You’ll be prompted to enter a question or statement for ChatGPT, and it will return a response.

### Example

```bash
Enter a prompt for ChatGPT: What are the uses of artificial intelligence in healthcare?
```

The response might look something like this:

```
ChatGPT response:
Artificial Intelligence (AI) is transforming healthcare by enabling faster diagnostics, personalized treatment plans, predictive analytics, robotic surgery, and improving patient outcomes through enhanced data analysis.
```

## Customization

You can modify parameters such as the model, maximum token length, and creativity (`temperature`) by adjusting the `get_chatgpt_response` function in the `chatgpt.py` script. Here's how:

- **`engine`**: Select the model (e.g., `"text-davinci-003"`).
- **`max_tokens`**: Limit the response length.
- **`temperature`**: Control the creativity of responses, with `0.0` being more precise and `1.0` being more random.

## Project Structure

```
openai-chatgpt-python/
├── chatgpt.py         # Main Python script for interacting with OpenAI API
├── README.md          # Project documentation
└── requirements.txt   # Python dependencies
```

## Dependencies

This project requires the following Python library:

- `openai`: The official Python package for communicating with OpenAI models.

You can install this and other dependencies by running:

```bash
pip install -r requirements.txt
```
