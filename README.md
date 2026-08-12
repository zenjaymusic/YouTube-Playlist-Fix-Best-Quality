# This script is now useless; YT fixed the bug.

>>>

# YouTube Playlist Fix + Best Quality

A Tampermonkey userscript that fixes broken playlist navigation in Opera GX and forces YouTube to always play at the highest available quality.

## What it does

- **Playlist fix** — forces a real page load on YouTube video links instead of relying on YouTube's internal AJAX navigation, which breaks playlist clicks in Opera GX
- **Best quality** — automatically sets playback to the highest available quality level on every video load

## Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/) for your browser
2. Click this link: [Install Script](https://github.com/zenjaymusic/YouTube-Playlist-Fix-Best-Quality/raw/refs/heads/main/YouTube%20Playlist%20Fix%20+%20Best%20Quality)
3. Click **Install** in the Tampermonkey prompt
4. Refresh YouTube

## Notes

- The playlist fix intercepts all `/watch` link clicks and converts them to hard navigations — this is intentional and is what resolves the Opera GX issue
- The quality fix runs on page load and after YouTube's internal navigation events, retrying for ~12 seconds to catch the player initialising
- Both fixes work independently — if you only need one, the other can be removed without breaking anything

## Browser support

Built for Opera GX but works on any Chromium-based browser with Tampermonkey installed.

## License

MIT — free to use, modify, and share.
