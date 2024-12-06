# mpd-url
Watch mpd queue for URLs that need to be fixed with yt-dlp

## Dependencies

This is a simple bash script that calls the following commands:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [mpc](https://github.com/MusicPlayerDaemon/mpc)
- [jq](https://github.com/jqlang/jq)
- awk, curl, diff, nc and other basics


## Usage

Create two services. The first is always running and the second is triggered by a periodic timer:

```sh

# Watch the mpd queue for changes
mpd-url watch

# Run periodically to replace any expired URLs in the mpd queue
mpd-url update

```
