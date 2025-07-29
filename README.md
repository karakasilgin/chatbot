# chatbot
# 🎵 FunBot: Your Discord Music & Game Companion

## About FunBot
FunBot is a versatile Discord bot designed to enhance your server experience with **music playback**, **interactive games**, and **engaging chat responses**. Whether you want to listen to your favorite tunes, challenge your friends to a number guessing game, or just have a casual chat, FunBot has you covered!

## ✨ Features

**🎵 Music Playback:**
* **`/play <song name/URL>`**: Play music directly from YouTube by searching or using a direct link.
* **`/skip`**: Skip the current song in the queue.
* **`/stop`**: Stop the music and clear the entire queue.
* **`/queue`**: Display the current music queue.

**🎮 Interactive Game:**
* **`/game`**: Start a fun **number guessing game** where you try to guess a secret number between 1 and 100 within a limited number of attempts.

**💬 Engaging Chat:**
* **Smart Replies**: FunBot can respond to common greetings ("hello," "hi," "hey"), questions ("how are you"), and appreciation ("thank you").
* **Contextual Help**: Ask "music," "song," "play," "game," or "help" for quick tips on how to use the bot.
* **`/chat <your message>`**: Initiate a direct conversation with the bot.

**⚙️ General Commands:**
* **`!ping`**: Check the bot's latency.

## 🚀 Getting Started

### Prerequisites
Before you can run FunBot, you'll need:
* **Python 3.8+** installed.
* A **Discord Bot Token**. You can get this by creating an application on the [Discord Developer Portal](https://discord.com/developers/applications).
* **FFmpeg** installed on your system. This is crucial for playing audio. You can download it from the [FFmpeg official website](https://ffmpeg.org/download.html).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/YourBotRepoName.git](https://github.com/YourUsername/YourBotRepoName.git)
    cd YourBotRepoName
    ```
2.  **Install the required Python libraries:**
    ```bash
    pip install -r requirements.txt
    ```
    *(You'll need to create a `requirements.txt` file containing `discord.py`, `youtube_dl`, and `pytube` if you decide to use it. For the provided code, `youtube_dl` and `discord.py` are the main ones.)*
    
    To generate `requirements.txt` from your environment:
    ```bash
    pip freeze > requirements.txt
    ```
    Alternatively, manually create `requirements.txt` with:
    ```
    discord.py==2.3.2 # Or your specific version
    youtube_dl # Or yt-dlp, if you prefer
    ```

3.  **Configure your Bot Token:**
    Open the `main.py` (or whatever you name your bot's main file) and replace `"YOUR_BOT_TOKEN"` with your actual Discord Bot Token.
    **Note:** It's highly recommended to use environment variables for your bot token instead of hardcoding it directly in the file for security reasons.
    
    *Example using an environment variable:*
    ```python
    import os
    # ...
    # Replace this line:
    # BOT_TOKEN = "YOUR_BOT_TOKEN"
    # with:
    BOT_TOKEN = os.getenv("DISCORD_BOT_TOKEN") 
    # And then run your bot with: DISCORD_BOT_TOKEN="YOUR_ACTUAL_TOKEN" python your_bot_file.py
    ```

4.  **Run the bot:**
    ```bash
    python your_bot_file_name.py
    ```

### Inviting the Bot to Your Server
To invite FunBot to your Discord server, you'll need the following permissions:
* `Read Messages/View Channels`
* `Send Messages`
* `Connect`
* `Speak`
* `Use Voice Activity`

You can generate an invite link from the [Discord Developer Portal](https://discord.com/developers/applications) under your bot's application settings.

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/YourUsername/YourBotRepoName/issues).

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
