# Discord Joker Bot

Is the repository for the JokerBot on my Discord server. Created using the medium version of Microsoft's DialoGPT iteration of GPT-2, this bot is live at my Discord server. Feel free to hop in and test it out. It does respond like Heath Ledger's Joker. XD

<a href="https://discord.gg/ACw4N66Fqf">Discord server invitation</a>

### How it works

I scourged Kaggle and Transcripts Wiki for the dataset I wanted. Finally used the transcript from The Dark Knight movie. I wanted to combine Joaquin Phoenix's Joker too, but being terrible at regex, could not parse the stuff properly. But will learn regex and come up with this version too, in JokerBotv2.

Moving on, after getting the dataset (uploaded on <a href="https://www.kaggle.com/sreyanghosh/dark-knight-dialogues">Kaggle</a>) I trained the DialoGPT model after creating basic context for Joker's Dialogues. I suggest using Colab since a pretty good GPU is required. After training the model, I uploaded it to Huggingface. Dataset creation is in joker_discBot.ipynb and model creation in joker_discBot_train.ipynb.

Huggingface serves as the platform on which my model is hosted. All requests are redirected here and responses relayed to Discord. After creating a Repl.it for the driver code (joker_bot_discord.py) I created an uptime bot that continuously serves the model even when the replit is offline. 

You can also test it out at my <a href="https://huggingface.co/sreyanghosh/DialoGPT-medium-joker">public Huggingface repo.</a>