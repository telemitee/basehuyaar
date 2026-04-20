.env
.cache
log.txt
.DS_Store
*.session
raw_files/
cache/
downloads/
__pycache__/
*.session-journal
FROM python:3.12-slim
RUN apt-get update &&
    apt-get install -y --no-install-recommends git ffmpeg curl unzip && \
    rm -rf /var/lib/apt/lis# Authored By Certified Coders © 2025
import re
from os import getenv
from dotenv import load_dotenv
from pyrogram import filters
# Load environment vabuild:
  docker:
    worker: Dockerfile
run:
  worker: bash startriables from .env file
load_dotenv()
# ── Core bot config ────────────────────────────────────────────────────────────
API_ID = int(getenv("API_ID", 27798659))
API_HASH = getenv("API_HASH", "26100c77cee02e5e34b2bbee58440f86")
BOT_TOKEN = getenv("BOT_TOKEN")
OWNER_ID = int(getenv("OWaiofiles
aiohttp
bing_image_downloader
bs4
deepaipython-3.12.6
edge-tts
ffmpeg-python
future
gitpython
google-api-python-client
gpytranslate
gtts
heroku3
httpx[http2]>=0.28.1
kurigram>=2.2.14
lexica-api
motor
nekosbest
numpy
opencv-python
pillow>=12.0.0
psutil
ntgcalls>=2.0.6
py-tgcalls>=2.2.8
pycryptodome
pydub
pyfiglet
qrcode
requests
speedtest-cli
SpeechRecognition
spotipy
telegraph
pytgcrypto
unidecode
yt-dlp[default]==2025.12.8
git+https://github.com/CertifiedCoders/youtube-search-pythonNER_ID", 7044783841))
OWNER_USERNAME = getenv("OWNER_USERNAME", "CertifiedCoder")
BOT_USERNAME = getenv("BOT_USERNAME", "AnnieXRobot")
BOT_NAME = getenv("BOT_NAME", "˹𝐀ɴɴɪᴇ ✘ 𝙼ᴜsɪᴄ˼ ♪")
ASSUSERNAME = getenv("ASSUSERNAME", "musicxannie")
# ── Database & logging ─────────────────────────────────────────────────────────
MONGO_DB_URI = getenv("MONGO_DB_URI")
LOGGER_ID = int(getenv("LOGGER_ID", -1002014167331))
# ── Limits (durations in min/sec; sizes in bytes) ──────────────────────────────
DURATION_LIMIT_MIN = int(getenv("DURATION_LIMIT", 300))
SONG_DOWNLOAD_DURATION = int(getenv("SONG_DOWNLOAD_DURATION", "1200"))
SONG_DOWNLOAD_DURATION_LIMIT = int(getenv("SONG_DOWNLOAD_DURATION_LIMIT", "1800"))
TG_AUDIO_FILESIZE_LIMIT = int(getenv("TG_AUDIO_FILESIZE_LIMIT", "157286400"))
TG_VIDEO_FILESIZE_LIMIT = int(getenv("TG_VIDEO_FILESIZE_LIMIT", "1288490189"))
PLAYLIST_FETCH_LIMIT = int(getenv("PLAYLIST_FETCH_LIMIT", "30"))
# ── External APIs ──────────────────────────────────────────────────────────────
COOKIE_URL = getenv("COOKIE_URL")  # required (paste link)
API_URL = getenv("API_URL")        # optional
VIDEO_API_URL = getenv("VIDEO_API_URL")  # optional
API_KEY = getenv("API_KEY")        # optional
DEEP_API = getenv("DEEP_API")      # optionalloyment ───────────────────────────────────────────────────────
HEROKU_APP_NAME = getenv("HEROKU_APP_NAME")
HEROKU_API_KEY = getenv("HEROKU_API_KEY")

# ── Git / updates ──────────────────────────────────────────────────────────────
UPSTREAM_REPO = getenv("UPSTREAM_REPO", "https://github.com/CertifiedCoders/AnnieXMusic")
UPSTREAM_BRANCH = getenv("UPSTREAM_BRANCH", "Master")
GIT_TOKEN = getenv("GIT_TOKEN")  # needed if repo is private

# ── Support links ──────────────────────────────────────────────────────────────
SUPPORT_CHANNEL = getenv("SUPPORT_CHANNEL", "https://t.me/CertifiedNetwork")
SUPPORT_CHAT = getenv("SUPPORT_CHAT", "https://t.me/CertifiedDiscussion")

# ── Assistant auto-leave ───────────────────────────────────────────────────────
AUTO_LEAVING_ASSISTANT = False
AUTO_LEAVE_ASSISTANT_TIME = int(getenv("ASSISTANT_LEAVE_TIME", "3600"))
# ── Debug ──────────────────────────────────────────────────────────────────────
DEBUG_IGNORE_LOG = True
# ── Spotify (optional) ─────────────────────────────────────────────────────────
SPOTIFY_CLIENT_ID = getenv("SPOTIFY_CLIENT_ID", "22b6125bfe224587b722d6815002db2b")
SPOTIFY_CLIENT_SECRET = getenv("SPOTIFY_CLIENT_SECRET", "c9c63c6fbf2f467c8bc68624851e9773")

# ── Session strings (optional) ─────────────────────────────────────────────────
STRING1 = getenv("STRING_SESSION")
STRING2 = getenv("STRING_SESSION2")
STRING3 = getenv("STRING_SESSION3")
STRING4 = getenv("STRING_SESSION4")
STRING5 = getenv("STRING_SESSION5")
# ── Media assets ───────────────────────────────────────────────────────────────
START_VIDS = [
    "https://telegra.ph/file/9b7e1b820c72a14d90be7.mp4",
    "https://telegra.ph/file/72f349b1386d6d9374a38.mp4",
    "https://telegra.ph/file/a4d90b0cb759b67d68644.mp4",
]
STICKERS = [
    "CAACAgUAAx0Cd6nKUAACASBl_rnalOle6g7qS-ry-aZ1ZpVEnwACgg8AAizLEFfI5wfykoCR4h4E",
    "CAACAgUAAx0Cd6nKUAACATJl_rsEJOsaaPSYGhU7bo7iEwL8AAPMDgACu2PYV8Vb8aT4_HUPHgQ",
]
HELP_IMG_URL = "https://files.catbox.moe/yg2vky.jpg"
PING_VID_URL = "https://files.catbox.moe/3ivvgo.mp4"
PLAYLIST_IMG_URL = "https://files.catbox.moe/yhaja5.jpg"
STATS_VID_URL = "https://telegra.ph/file/e2ab6106ace2e95862372.mp4"
TELEGRAM_AUDIO_URL = "https://files.catbox.moe/mlztag.jpg"
TELEGRAM_VIDEO_URL = "https://files.catbox.moe/tiss2b.jpg"
STREAM_IMG_URL = "https://files.catbox.moe/1d3da7.jpg"
SOUNCLOUD_IMG_URL = "https://files.catbox.moe/zhymxl.jpg"
YOUTUBE_IMG_URL = "https://files.catbox.moe/veykzq.jpg"
SPOTIFY_ARTIST_IMG_URL = SPOTIFY_ALBUM_IMG_URL = SPOTIFY_PLAYLIST_IMG_URL = YOUTUBE_IMG_URL

# ── Helpers ────────────────────────────────────────────────────────────────────
def time_to_seconds(time: str) -> int:
    return sum(int(x) * 60**i for i, x in enumerate(reversed(time.split(":"))))

DURATION_LIMIT = time_to_seconds(f"{DURATION_LIMIT_MIN}:00")



    "ʜᴇʟʟᴏ {0}, 🥀\n\n ɪᴛ'ꜱ ᴍᴇ {1} !\n\n┏━━━━━━━━━━━━━━━━━⧫\n┠ ◆ ꜱᴜᴘᴘᴏʀᴛɪɴɢ ᴘʟᴀᴛꜰᴏʀᴍꜱ : ʏᴏᴜᴛᴜʙᴇ, ꜱᴘᴏᴛɪꜰʏ,\n┠ ◆ ʀᴇꜱꜱᴏ, ᴀᴘᴘʟᴇᴍᴜꜱɪᴄ , ꜱᴏᴜɴᴅᴄʟᴏᴜᴅ ᴇᴛᴄ.\n┗━━━━━━━━━━━━━━━━━⧫\n┏━━━━━━━━━━━━━━━━━⧫\n┠ ➥ Uᴘᴛɪᴍᴇ : {2}\n┠ ➥ SᴇʀᴠᴇʀSᴛᴏʀᴀɢᴇ : {3}\n┠ ➥ CPU Lᴏᴀᴅ : {4}\n┠ ➥ RAM Cᴏɴsᴜᴘᴛɪᴏɴ : {5}\n┠ ➥ ᴜꜱᴇʀꜱ : {6}\n┠ ➥ ᴄʜᴀᴛꜱ : {7}\n┗━━━━━━━━━━━━━━━━━⧫\n\n🫧 ᴅᴇᴠᴇʟᴏᴩᴇʀ 🪽 ➪ [ᴄᴇʀᴛɪғɪᴇᴅ ᴄᴏᴅᴇʀ ✔︎](https://t.me/CertifiedCoder)",
    "ʜɪɪ, {0} ~\n\n◆ ɪ'ᴍ ᴀ {1} ᴛᴇʟᴇɢʀᴀᴍ ꜱᴛʀᴇᴀᴍɪɴɢ ʙᴏᴛ ᴡɪᴛʜ ꜱᴏᴍᴇ ᴜꜱᴇꜰᴜʟ\n◆ ᴜʟᴛʀᴀ ғᴀsᴛ ᴠᴄ ᴘʟᴀʏᴇʀ ꜰᴇᴀᴛᴜʀᴇꜱ.\n\n✨ ꜰᴇᴀᴛᴜʀᴇꜱ ⚡️\n◆ ʙᴏᴛ ғᴏʀ ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘs.\n◆ Sᴜᴘᴇʀғᴀsᴛ ʟᴀɢ Fʀᴇᴇ ᴘʟᴀʏᴇʀ.\n◆ ʏᴏᴜ ᴄᴀɴ ᴘʟᴀʏ ᴍᴜꜱɪᴄ + ᴠɪᴅᴇᴏ.\n◆ ʟɪᴠᴇ ꜱᴛʀᴇᴀᴍɪɴɢ.\n◆ ɴᴏ ᴘʀᴏᴍᴏ.\n◆ ʙᴇꜱᴛ ꜱᴏᴜɴᴅ Qᴜᴀʟɪᴛʏ.\n◆ 24×7 ʏᴏᴜ ᴄᴀɴ ᴘʟᴀʏ ᴍᴜꜱɪᴄ.\n◆ ᴀᴅᴅ ᴛʜɪꜱ ʙᴏᴛ ɪɴ ʏᴏᴜʀ ɢʀᴏᴜᴘ ᴀɴᴅ ᴍᴀᴋᴇ ɪᴛ ᴀᴅᴍɪɴ ᴀɴᴅ ᴇɴᴊᴏʏ ᴍᴜꜱɪᴄ 🎵.\n\n┏━━━━━━━━━━━━━━━━━⧫\n┠ ◆ ꜱᴜᴘᴘᴏʀᴛɪɴɢ ᴘʟᴀᴛꜰᴏʀᴍꜱ : ʏᴏᴜᴛᴜʙᴇ, ꜱᴘᴏᴛɪꜰʏ,\n┠ ◆ ʀᴇꜱꜱᴏ, ᴀᴘᴘʟᴇᴍᴜꜱɪᴄ , ꜱᴏᴜɴᴅᴄʟᴏᴜᴅ ᴇᴛᴄ.\n┗━━━━━━━━━━━━━━━━━⧫\n┏━━━━━━━━━━━━━━━━━⧫\n┠ ➥ Uᴘᴛɪᴍᴇ : {2}\n┠ ➥ SᴇʀᴠᴇʀSᴛᴏʀᴀɢᴇ : {3}\n┠ ➥ CPU Lᴏᴀᴅ : {4}\n┠ ➥ RAM Cᴏɴsᴜᴘᴛɪᴏɴ : {5}\n┠ ➥ ᴜꜱᴇʀꜱ : {6}\n┠ ➥ ᴄʜᴀᴛꜱ : {7}\n\n\n🫧 ᴅᴇᴠᴇʟᴏᴩᴇʀ 🪽 ➪ 
# ── Runtime structures ─────────────────────────────────────────────────────────
BANNED_USERS = filters.user()
adminlist, lyrical, autoclean, confirmer = {}, {}, [], {}

# ── Minimal validation ─────────────────────────────────────────────────────────
if SUPPORT_CHANNEL and not re.match(r"^https?://", SUPPORT_CHANNEL):
    raise SystemExit("[ERROR] - Invalid SUPPORT_CHANNEL URL. Must start with https://")

if SUPPORT_CHAT and not re.match(r"^https?://", SUPPORT_CHAT):
    raise SystemExit("[ERROR] - Invalid SUPPORT_CHAT URL. Must start with https://")ts/* && \
    curl -fsSL https://deno.land/install.sh | sh && \
    ln -s /root/.deno/bin/deno /usr/local/bin/deno

WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -U pip && \
    pip install --no-cache-dir -r requirements.txt

COPY . .
CMD ["python3", "-m", "AnnieXMedia"]
MIT License

Copyright (c) 2025 Certified Coder
API_ID=              # Required - Get from https://my.telegram.org
API_HASH=            # Required - From https://my.telegram.org
BOT_TOKEN=           # Required - Get t.me/BotFather
OWNER_ID=            # Required - Your Telegram user ID
LOGGER_ID=           # Required - Log group/channel ID
STRING_SESSION=      # Required - Generate from @SessionBuilderbot
MONGO_DB_URI=        # Required - MongoDB connection string
COOKIE_URL=          # Required - YT Cookies url

DEEP_API=            # Optional - Get from https://deepai.org
API_KEY=             # Optional - External API key for song Download
VIDEO_API_URL=       # Optional - External API url for video Download
API_URL=             # Optional - External API url for audio Download

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without res# sᴇᴄᴜʀɪᴛʏ ᴘᴏʟɪᴄʏ

## sᴜᴘᴘᴏʀᴛᴇᴅ ᴠᴇʀsɪᴏɴs

ʙᴇʟᴏᴡ ᴛᴀʙʟᴇ shows ᴡʜɪᴄʜ ᴠᴇʀsɪᴏɴ ɪs sᴛᴀʙʟᴇ ᴀɴᴅ sᴇᴄᴜʀɪᴛʏ ᴜᴘᴅᴀᴛᴇᴅ ᴀɴᴅ ᴡʜɪᴄʜ ɪs ɴᴏᴛ
| Version | Supported |
| :-----: | :-------: |
|   1.0   |     ❌     |
|   2.0   |     ❌     |
|   2.1   |     ❌     |{
  "name": "ANNIE X MUSIC",
  "description": "ANNIE X MUSIC is a powerful and versatile Telegram Music Player Bot built with Python, utilizing Pyrogram and Py-Tgcalls libraries for high-quality group voice chat music streaming. This bot offers seamless playback, custom download server integration, and AI-enhanced features for a premium user experience.",
  "logo": "https://telegra.ph/file/2c6d1a6f78eba6199933a.jpg",
  "keywords": [
    "python3",
    "telegram",
    "music-bot",
    "pyrogram",
    "py-tgcalls",
    "AnnieXMusic"
  ],
  "env": {
    "API_ID": {
      "description": "Telegram API ID, available at https://my.telegram.org. Required to connect the bot to Telegram servers.",
      "required": true,
      "value": ""
    },
    "API_HASH": {
      "description": "Telegram API Hash, available at https://my.telegram.org. Required alongside API ID.",
      "required": true,
      "value": ""
    },
    "BOT_TOKEN": {
      "description": "Bot Token from BotFather after creating your Telegram bot.",
      "required": true,
      "value": ""
    },
    "MONGO_DB_URI": {
      "description": "MongoDB database connection URI, used for storing user and bot-related data. Get it from https://cloud.mongodb.com.",
      "required": true,
      "value": ""
    },
    "OWNER_ID": {
      "description": "Your Telegram numeric user ID (use @userinfobot to find it). Multiple IDs can be separated by a space.",
      "required": true,
      "value": ""
    },
    "STRING_SESSION": {
      "description": "Pyrogram v2 session string. Generate it securely from https://telegram.tools/session-string-generator#pyrogram.",
      "value": "",
      "required": true
    },
    "LOGGER_ID": {
      "description": "Chat ID of your log group where the bot sends important logs. Make sure the bot is admin in that group.",
      "required": true,
      "value": ""
    },
    "COOKIE_URL": {
      "description": "Direct raw link (from Batbin or Pastebin) to your YouTube cookies.txt file for better download support.",
      "required": true,
      "value": ""
    },
    "API_URL": {
      "description": "(Optional) URL of a custom API server used for music downloads or other services.",
      "required": false,
      "value": ""
    },
    "VIDEO_API_URL": {
      "description": "(Optional) URL of a custom API server used for video downloads or other services.",
      "required": false,
      "value": ""
    },
    "API_KEY": {
      "description": "(Optional) API Key associated with your custom music download server (used with API_URL).",
      "required": false,
      "value": ""
    },
    "DEEP_API": {
      "description": "(Optional) DeepAI API key for enabling AI-powered features. Get it from https://deepai.org/.",
      "required": false,
      "value": ""
    },
    "HEROKU_API_KEY": {
      "description": "Your Heroku account API key, required if you want the bot to support auto-updates or dynamic deployments.",
      "required": false,
      "value": ""
    },
    "HEROKU_APP_NAME": {
      "description": "The name of your Heroku app. Required if using HEROKU_API_KEY for deployments.",
      "required": false,
      "value": ""
    }
  },
  "buildpacks": [
    {
      "url": "heroku/python"
    },
    {
      "url": "heroku/nodejs"
    },
    {
      "url": "https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.git"
    }
  ],
  "stack": "container"
}
|   2.2   |     ❌     |
|   2.3   |     ✅     |


## ʀᴇᴘᴏʀᴛɪɴɢ ᴀ ᴠᴜʟɴᴇʀᴀʙɪʟɪᴛʏ

ɪғ ʏᴏᴜ ᴡᴀɴᴛ ᴛᴏ ʀᴇᴘᴏʀᴛ ᴀ ᴍᴀᴊᴏʀ ᴏʀ ᴍɪɴᴏʀ ᴠᴜʟɴᴇʀᴀʙɪʟɪᴛʏ ғʀᴏᴍ ᴏᴜʀ ᴘʀᴏᴊᴇᴄᴛ?

ғɪʀsᴛ ᴏғ ᴀʟʟ ɪɴғᴏʀᴍ ᴛʜᴇ ᴏʀɪɢɪɴᴀʟ ᴄʀᴇᴀᴛᴏʀ ᴏғ ᴛʜᴇ ᴘᴀᴄᴋᴀɢᴇ ғʀᴏᴍ PyPi
ᴀɴᴅ ᴛʜᴇɴ ᴍᴀᴋᴇ ᴀ ɪssᴜᴇ ɪɴ ᴏᴜʀ ᴘʀᴏᴊᴇᴄᴛ.

## ᴀɴɴɪᴇ x ᴍᴜsɪᴄ ᴏᴡɴᴇʀ
- [ɢɪᴛʜᴜʙ](https://github.com/CertifiedCoders)
- [ᴛᴇʟᴇɢʀᴀᴍ](https://t.me/CertifiedCoder)
- [ sᴜᴘᴘᴏʀᴛ](https://t.me/CertifiedCoders)

## ɪɴғᴏ 
ᴛʜɪs ɪs **ᴀɴɴɪᴇ x ᴍᴜsɪᴄ** , ᴏᴩᴇɴ sᴏᴜʀᴄᴇ ᴛᴇʟᴇɢʀᴀᴍ ᴠᴄ ᴍᴜsɪᴄ ᴘʟᴀʏᴇʀ ʙᴏᴛ ᴡɪᴛʜ sᴏᴍᴇ ɢʀᴏᴜᴘ ᴍᴀɴᴀɢᴀᴇᴍᴇɴᴛ ғᴇᴀᴛᴜʀᴇs.

ᴡʀɪᴛᴛᴇɴ ɪɴ ᴩʏᴛʜᴏɴ ᴡɪᴛʜ ᴛʜᴇ ʜᴇʟᴩ ᴏғ : [ᴘʏᴛɢᴄᴀʟʟs](https://github.com/pytgcalls/pytgcalls), 
[ᴩʏʀᴏɢʀᴀᴍ](https://github.com/KurimuzonAkuma/pyrogram), 
[ʏᴛᴅʟᴘ](https://github.com/yt-dlp/yt-dlp), 
ᴀɴᴅ ᴜsɪɴɢ [ᴍᴏɴɢᴏ](https://cloud.mongodb.com) ᴀs ᴅᴀᴛᴀʙᴀsᴇ.

ʜᴇʀᴇ ɪs ᴍʏ sᴏᴜʀᴄᴇ ᴄᴏᴅᴇ : [ɢɪᴛʜᴜʙ-ʟɪɴᴋ](https://github.com/CertifiedCoders/AnnieXMusic)


ᴀᴠᴀ ʀᴏʙᴏᴛ ɪs ʟɪᴄᴇɴsᴇᴅ ᴜɴᴅᴇʀ ᴛʜᴇ [ᴍɪᴛ ʟɪᴄᴇɴsᴇ](https://github.com/CertifiedCoders/AnnieXMusic/blob/master/LICENSE).

© 2024 - 2025 [ᴅᴇᴠ](https://github.com/CertifiedCoders), ᴀʟʟ ʀɪɢʜᴛs ʀᴇsᴇʀᴠᴇᴅ.triction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
worker: bash start
