# skeptical-x-original-media-fetch (Grok skill)

Fetch original-resolution photos and videos from X posts with no API: fxtwitter JSON for media URLs, then `?name=orig` on pbs.twimg.com.

## Install

This repo is the skill folder: `SKILL.md` sits at the top level. Clone it into a skills directory.

User scope (all your projects), macOS or Linux:

    mkdir -p ~/.grok/skills
    git clone https://github.com/skeptical-agency/skeptical-x-original-media-fetch.git ~/.grok/skills/skeptical-x-original-media-fetch

User scope, Windows PowerShell (assumes Grok reads skills from `$HOME\.grok\skills`):

    New-Item -ItemType Directory -Force "$HOME\.grok\skills"
    git clone https://github.com/skeptical-agency/skeptical-x-original-media-fetch.git "$HOME\.grok\skills\skeptical-x-original-media-fetch"

Project scope (shared via git):

    mkdir -p .grok/skills
    git clone https://github.com/skeptical-agency/skeptical-x-original-media-fetch.git .grok/skills/skeptical-x-original-media-fetch

No git? Download the repo as a zip from GitHub and unzip it into a folder named `skeptical-x-original-media-fetch` inside the skills directory.

More skills: [skeptical-agency/grok-skills](https://github.com/skeptical-agency/grok-skills).

## Requirements

- `curl`, Python 3 and `ffprobe` (from ffmpeg) on your PATH; `yt-dlp` for the Facebook/TikTok tip
- macOS: `brew install yt-dlp ffmpeg`
- Linux: `pipx install yt-dlp` and `sudo apt install ffmpeg`
- Windows: `winget install yt-dlp.yt-dlp` and `winget install Gyan.FFmpeg`, then open a new terminal

## Use

Ask Grok things like:

> get the original resolution photo from this X post: <url>

SKILL.md has a plain-English intro, a worked example, the exact commands and the known pitfalls.

## Responsible use

Only fetch and use media you have the rights to use. Respect each platform's terms and the poster's copyright. This relies on a third-party mirror that can change at any time.

## License

MIT, see LICENSE.
