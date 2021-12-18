<h1 align="center">SaveMedia</h1>

<p align="center">The collection of scripts for yt-dlp.</p>

Based on [TheFrenchGhostys-YouTube-DL-Archivist-Scripts](https://github.com/TheFrenchGhosty/TheFrenchGhostys-YouTube-DL-Archivist-Scripts), this project focuses on archiving.

Added downloading comments in everything, added downloading all subtitles (useful to search media by text), removed the watch scripts (use the original scripts for downloading specifically to watch, or visit multimedia sites with [TarTube](https://github.com/axcore/tartube), or ), simplified the directory structure.

The recent scripts uses same sources as the archivist scripts.

## Features:

- Download content in the best possible quality, better than every other software, period
- Download all kind of content: channels, playlists and individual videos
- Download audio only (especially useful when no much disk space), in the best possible quality
- Download subtitles (including autogenerated) and comments
- Easily expandable for users familiar with yt-dlp / youtube-dl
- [SponsorBlock](https://sponsor.ajay.app/) integration using [mpv_sponsorblock](https://github.com/po5/mpv_sponsorblock) by [@po5](https://github.com/po5)
- [Jellyfin](https://jellyfin.org/) integration using [Jellyfin YouTube Metadata Plugin](https://github.com/ankenyr/jellyfin-youtube-metadata-plugin) by [@ankenyr](https://github.com/ankenyr)

---

## Installation (Linux, macOS):

Install [yt-dlp](https://github.com/yt-dlp/yt-dlp) and [ffmpeg](https://www.ffmpeg.org/) (optionally, install [atomicparsley](https://github.com/wez/atomicparsley), it's required for embedding thumbnails into m4a files).

---

## Installation (Windows):

The Windows version, while it existed, required a lot of work to maintain because it needed specific changes compared to the linux version, and was never extensively tested. Windows users need to use the scripts in WSL, Cygwin, Git Bash, or some other Linux-on-Windows environment that enables Bash functionality in Windows.
 
Installation using WSL (recommended): [Here](docs/WSL.md)

Installation using Cygwin, Git Bash or similar: [Here](docs/Cygwin-Git-Bash.md)

Downloaded videos will likely exceed Windows' 260-character path length limit and not be playable out of the box. You should read more about [paths](docs/About-Paths.md) to familiarize yourself with the issue, as well as some potential workarounds.

---

## Usage: 

Create a folder where you want your videos downloaded in a drive where you have enough space available.

Put the folders `Channels`, `Playlists`, `Unique` and `Audio` in the created folder (See the documentation to understand the differences).

Add content to a 'Source - XXXXXX.txt' (or 'Audio - XXXXXX.txt') file depending of what type of content you want to download (See the documentation to understand the differences).

Open a terminal in the folder of the script you want to use and run `./save` or `./save_recent`.

Done.

---

## Documentation:

- Scripts Type (Archivist, Audio): [Here](docs/Scripts-Type.md)

- Content Type (Channels, Playlists, Unique): [Here](docs/Content-Type.md)

- SponsorBlock implementation: [Here](docs/SponsorBlock.md)

- Region Restriction: [Here](docs/Region-Restriction.md)

- Details: [Here](docs/Details.md) 

---

## Related Projects:

- [SaveSites](https://github.com/defder-su/SaveSites)

- [RatBrowser](https://ratbrowser.com)

- [IPFS](https://ipfs.io)

- [ZeroNet](https://zeronet.io)

---

## Contact:

You are welcome in [Defder.SU](https://defder.su).
