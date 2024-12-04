# mpd-url
Watch mpd queue for URLs that need to be fixed with yt-dlp

## Dependencies

This is a simple bash script that calls the following commands:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [mpc](https://github.com/MusicPlayerDaemon/mpc)
- [jq](https://github.com/jqlang/jq)
- nc, awk, curl, and other basics


## Usage

Create two services: one that is always running and another that is triggered by a periodic timer.

```sh

# Watch the mpd queue for changes
mpd-url watch

# Check the queue for any expired URLs and replace them
mpd-url update

```
