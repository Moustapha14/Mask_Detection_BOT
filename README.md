
# Mask Detection Bot

Welcome to the Mask Detection Bot project. This initiative utilizes a powerful deep learning model to detect whether individuals in photos are wearing masks. The bot is implemented via Telegram for ease of access and use from anywhere in the world.

## Project Overview

In the current global climate, wearing masks is a crucial preventive measure against the spread of certain airborne illnesses. This project contributes to these efforts by making mask detection as easy as sending a photo. Simply send an image to this Telegram bot, and it will tell you whether the subjects are wearing masks.

## Features

- **Image Analysis**: Upload images directly through a Telegram chat, and receive immediate feedback on whether people in the pictures are wearing masks.
- **Deep Learning Power**: Uses the latest `fastai` model for accurate predictions.
- **Ease of Access**: Accessible anytime through Telegram, a platform used worldwide.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- Telegram Bot API
- PyTorch, fastai, and other relevant Python libraries

### Installation

1. Clone the repository to your local machine:

```bash
git clone <URL-of-this-repo>
```

2. Navigate to the project directory:

```bash
cd path/to/Mask-Detection-Bot
```

3. Install the necessary Python packages and dependencies using pip. Given that specific package versions are necessary, we'll need to install them from a requirements file or individually. This project specifically requires certain versions of `fastai`, `torch`, and `torchvision`.

```bash
pip install python-telegram-bot
pip install fastai==2.0.13
pip install torch==1.6.0+cpu -f https://download.pytorch.org/whl/torch_stable.html
pip install torchvision==0.7.0+cpu
pip install ipython
```

### Setup

1. Create a bot on Telegram:
   - Talk to @BotFather on Telegram. Use the `/newbot` command to create a new bot and obtain a token for the HTTP API.
   - Follow the instructions, give your bot a name, and receive your TOKEN.

2. Update the `bot.py` file (or the main script you use) with your bot token.

```python
updater = Updater(token='YOUR_TOKEN_HERE', use_context=True)
```

## Running the Bot

1. To start the bot, run the main script:

```bash
python bot.py
```

2. Open your Telegram application and search for the bot you created using @BotFather. Start a conversation and try sending a photo to see if people are wearing masks.

## Usage

- Send a `/start` command to activate the bot.
- Upload an image or send an image URL, and the bot will analyze the photo to detect masks.
- The bot will respond with the detection results.

