

<p align="center">
<a href="https://dashboard.heroku.com/new?template=https://github.com/Silenthrax/YOUTUBE"><img src="https://img.shields.io/badge/Deploy%20To%20Heroku-purple?style=for-the-badge&logo=heroku&logoColor=white" width="250px" alt="Deploy to Heroku"></a>
</p>

<h2 align="center">🚀 Deploy to Render (Free)</h2>

<p align="center">
  <a href="https://render.com/deploy?repo=https://github.com/Silenthrax/YOUTUBE">
    <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
  </a>
</p>

## ✨ Features

- **Play Music**: Stream high-quality music in Telegram voice chats
- **Multiple Sources**: YouTube, Spotify, SoundCloud, and local files
- **Playlists**: Create and manage playlists for your group
- **Multi-Language**: Available in multiple languages
- **Elegant UI**: Clean and modern user interface
- **Group Management**: Powerful admin commands
- **High Quality**: Crystal clear audio streaming

## 🔥 Essential Commands

| Command | Description |
| --- | --- |
| `/play` | Play song from YouTube |
| `/pause` | Pause the current stream |
| `/resume` | Resume the paused stream |
| `/skip` | Skip to the next song |
| `/stop` | Stop the streaming |
| `/playlist` | Show the playlist |
| `/song` | Download a song as audio |
| `/settings` | Open bot settings |

## 🚀 Deployment Guide

### 🔧 VPS Deployment (Step by Step)

#### Prerequisites

First, update your system and install required packages:

```bash
sudo apt-get update && sudo apt-get upgrade -y
```

# Install Python, Pip, FFmpeg, Git, Screen, Node.js, npm


```bash
sudo apt-get install python3 python3-pip ffmpeg git screen curl -y
```

# Install Node.js (LTS Version) and npm


```bash
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
```

```bash
sudo apt-get install -y nodejs
```


#### Clone the Repository


```bash
git clone https://github.com/NoxxOP/ShrutiMusic
cd ShrutiMusic
```

#### Run 24x7 bot using screen 


```bash
screen 
```


#### Setup Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

#### Install Dependencies

```bash
pip3 install -U pip
pip3 install -U -r requirements.txt
```

#### Configuration

Copy example config file and edit it with your values:

```bash
nano .env
```
Fill in your:
- `API_ID` & `API_HASH` from my.telegram.org  
- `BOT_TOKEN` from @BotFather  
- `MONGO_DB_URI` from your MongoDB Atlas cluster  
- `OWNER_ID` (Your Telegram user ID)  
- `OWNER_USERNAME` (Your Telegram username without @)  
- `BOT_USERNAME` (Your bot’s username without @)  
- `UPSTREAM_REPO` (GitHub repo URL for updates Recommend : Original Source)  
- `STRING_SESSION` (Generate using @ShrutiSessionBot)  
- `GIT_TOKEN` (If your repo is private)  
- `LOG_GROUP_ID` (Log group/channel ID starting with -100)  
- `SUPPORT_GROUP` (Full Link of your Support Group)  
- `SUPPORT_CHANNEL` (Full Link Of your Support channel )  
- `COOKIE_URL` (Optional: If no cookies file in Your Repo)  
- `START_IMG_URL` (Image URL for /start message thumbnail)

#### Starting the Bot

There are two ways to start the bot:

1. Using Python directly:
```bash
python3 -m ShrutiMusic
```

2. Using Bash script:
```bash
bash start
```

To detach the screen, press `Ctrl+A` then `D`

To reattach the screen later:

```bash
screen -ls
```
See Your Screen ID and then:

```bash
screen -r {screen_id}
```

Make Sure Fill Your Screen ID without Bracket {} .
Example : screen -r 108108

### ☁️ Heroku Deployment

<p align="center">
<a href="https://dashboard.heroku.com/new?template=https://github.com/Silenthrax/YOUTUBE"><img src="https://img.shields.io/badge/Deploy%20To%20Heroku-purple?style=for-the-badge&logo=heroku&logoColor=white" width="250px" alt="Deploy to Heroku"></a>
</p>

1. Click the button above
2. Fill in the required details:
   - App name
   - API_ID & API_HASH
   - BOT_TOKEN
   - MUSIC_BOT_NAME
   - SESSION_STRING
   - SUDO_USERS (your User ID)
3. Click "Deploy App"
4. Once deployed, go to Resources tab and turn on the worker

