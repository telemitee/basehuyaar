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

RUN apt-get update && \
    apt-get install -y --no-install-recommends git ffmpeg curl unzip && \
    rm -rf /var/lib/apt/lists/* && \
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
