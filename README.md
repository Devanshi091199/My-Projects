# LLM ChatHub

## Introduction
LLM ChatHub is a powerful and flexible chatbot application designed to integrate various Large Language Models (LLMs). This project allows users to interact with open-source or custom-trained models effortlessly through a user-friendly interface. It supports multiple deployment options, including a web-based Gradio application and a Discord bot.

## Author
**Developed by Devanshi Srivastava**

## Features
- Supports multiple LLMs from Hugging Face's `transformers` library.
- User-friendly Gradio-based UI for seamless interactions.
- Discord Bot integration for interactive conversations.
- Internet search capability using Serper API.
- Options to use pre-trained models or custom models.
- Efficient conversation and context management.
- Easy deployment and local execution.

## Installation
To set up the project on your local machine:

```sh
git clone <repository_url>
cd LLM-ChatHub
python -m venv venv
source venv/bin/activate   # On Windows use 'venv\Scripts\activate'
pip install -r requirements.txt
```

## Usage
### Running the Gradio Application
Run the following command to start the chatbot UI:

```sh
python app.py
```

Once the server starts, open `http://127.0.0.1:6006` in your browser to interact with the chatbot.

### Running the Discord Bot
To deploy the chatbot as a Discord bot, run:

```sh
python discord_app.py --token "YOUR_DISCORD_BOT_TOKEN" --model-name "alpaca-lora-7b" --max-workers 1 --mode-full-gpu --local-files-only
```

You'll need to generate a Discord bot token from the [Discord Developer Portal](https://discord.com/developers/docs/intro).

## Custom Model Integration
If you want to use your own model, make sure it's compatible with Hugging Face's `transformers` library and provide the correct model path in the UI.

## Internet Search Support
To enable internet search capability, get a free **Serper API Key** from [serper.dev](https://serper.dev/) and pass it as a parameter:

```sh
python app.py --serper-api-key "YOUR_SERPER_API_KEY"
```

## Supported Models
LLM ChatHub supports multiple fine-tuned instruction-based models, including:
- **Alpaca-LoRA** (7B, 13B, 30B, 65B)
- **StableLM**
- **KoAlpaca**
- **Flan-Alpaca**
- **MPT Chat Models**
- **Falcon-7B, Falcon-40B**
- **Vicuna, Guanaco, WizardLM, and many more!**

## Contribution
Contributions are welcome! Feel free to fork this repository and create pull requests.

## License
This project is licensed under the MIT License.

---
Developed with ❤️ by **Devanshi Srivastava**
