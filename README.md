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
|   2.1   |     ❌     |
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
