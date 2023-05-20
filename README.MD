Welcome to the Suprebot chatbot for Telegram, inspired by the virtual assistant J.A.R.V.I.S. from the Marvel universe. 



## Requirements
To use Suprebot, you will need a Telegram bot, OpenAI API access token, and python3 installed. Ensure that the `OPENAI_TOKEN` and `TELEGRAM_TOKEN` environment variables are set with your respective credentials.

You may also need to install ffmpeg (ubuntu example)
```
sudo apt-get -y update
sudo apt-get install -y ffmpeg
```

## Getting started
Follow the steps below to get started:

Clone the repository using the command: 
```
git clone git@github.com:SupreLTD/Suprebot.git
```

Navigate to your project folder and install dependencies using pip:
```
pip install --upgrade pip
pip install -r requirements.txt
```

 Run the command to start the bot.
```
python3 bot.py
```

Alternatively, if you have Docker installed, you can run Suprebot inside a Docker container by following these instructions:

Build the bot image using the Dockerfile located in the project root folder with this command: 
```
docker build -t suprebot .
```

Run the bot container ensuring you specify your OpenAI and Telegram tokens: 
```
docker run -d -e OPENAI_TOKEN=<your_openai_token> -e TELEGRAM_TOKEN=<your_telegram_token> suprebot
```

## Schrodinger`s Live Demo
You can see a live demo of suprebot by sending `/help` to `@SupreLTD_bot` on Telegram. Note that the bot might or might not be running due to its limited budget for accessing OpenAI`s APIs.