MusicBot README
Introduction

This Discord MusicBot allows users to play music from YouTube and other supported sites directly in a Discord voice channel. It supports various commands for music playback, such as play, pause, skip, and volume control.
Prerequisites

    Python 3.6 or higher
    discord.py library
    yt-dlp library
    A Discord bot token

Setup

    Environment Setup:
        Install the required Python packages using pip:

    pip install -U discord.py yt-dlp python-dotenv

Bot Token:

    Create a file named Token.env in your project directory.
    Place your Discord bot token in the file like this:

    makefile

        DISCORD_TOKEN=your_bot_token_here

    Bot Permissions:
        Make sure your bot has permissions to join and speak in voice channels.

Running the Bot

    Start the Bot:
        Run the script using Python:

        python3 your_script_name.py

    Invite the Bot to Your Server:
        Use the Discord developer portal to invite your bot to the server.

Usage

    Join a Voice Channel:
    /join - The bot joins the voice channel you are currently in.

    Play Music:
    /play [song name or URL] - Plays the specified song. If a song is already playing, the new song will be added to the queue.

    Pause/Resume:
    /pause - Pauses the current song.
    /resume - Resumes the paused song.

    Skip Song:
    /skip - Skips the current song. If used by the song requester, it skips immediately. Otherwise, it requires votes.

    Volume Control:
    /volume [0-100] - Sets the playback volume.

    Queue Management:
    /queue - Displays the current song queue.
    /shuffle - Shuffles the song queue.
    /remove [index] - Removes a song from the queue at the specified index.

    Looping:
    /loop - Toggles looping of the current song.

    Leaving the Channel:
    /leave - Stops the music and makes the bot leave the voice channel.

Additional Information

    Ensure your Discord bot has the necessary permissions to read messages, connect to voice channels,speak, message content intent, server members intent and presence intent.
    
