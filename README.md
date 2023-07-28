# Telegram Chatbot with OpenAI Integration

This repository contains a Python script for a Telegram chatbot integrated with OpenAI for generating responses. The chatbot is built using the Telegram Bot API and utilizes OpenAI's powerful language model to generate contextually relevant responses.

## Prerequisites

Before running the chatbot, make sure you have the following:

1. Python 3.x installed on your system.
2. OpenAI API Key: Sign up for an account on [OpenAI](https://openai.com) and get your API key.
3. Telegram Bot Token: Create a new bot on Telegram and obtain the API token for your bot. You can find more information on how to create a bot and get its token in the [Telegram Bot Documentation](https://core.telegram.org/bots#botfather).

## Installation

1. Clone this repository to your local machine using the following command:

```bash
git clone https://github.com/karansinghkushwah1/Chatgpt_Telegram_bot.git
```
2. Install the required Python packages by running:
```bash
pip install python-telegram-bot openai
```
## Configuration
1. Open the bot.py file in your preferred text editor.
2. Replace 'Your_token' in the TOKEN variable with your Telegram bot token obtained from BotFather.
3. Replace 'Your_bot_username' in the BOT_USERNAME variable with your bot's username without the '@' symbol.
4. Replace 'Your_OpenAi_API_Key' with your OpenAI API key.

## How to Use
1. Run the bot by executing the following command in your terminal:
```bash
python main.py
```

1. Once the bot is running, open your Telegram app and find your bot using the username you set earlier.
2. Start a chat with the bot and type any message.
3. The bot will respond with a contextually generated message using the OpenAI language model.
   
## Commands
The chatbot responds to the following commands:

1. /start: Initiates a conversation with the bot.
2. /help: Displays a help message guiding users on how to interact with the bot.
3. /custom: Responds with a custom message. You can customize the response in the custom_command function in the script.

## How the Bot Works

1. When a user sends a message to the bot, it logs the message in the console.
2. The bot uses the handle_message function to process incoming messages and generate responses.
3. If the user's message is a reply to the bot's previous message, the bot processes the message and generates a response using the OpenAI API.
4. If the message is a mention in a group or supergroup, the bot extracts the relevant text and generates a response.
5. If the message is a regular text message in a private chat, the bot directly generates a response using the OpenAI API.
6. The bot sends the generated response back to the user.

## Error Handling
The bot includes a basic error handler, which logs any errors that occur during execution. If an error occurs, the bot will log the error and continue running.

## Disclaimer
This is a simple example of how to build a Telegram chatbot using Python and integrate it with OpenAI. The OpenAI API key and Telegram bot token should be kept private and not shared publicly.
