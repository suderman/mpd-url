# mpd-url
Watch mpd queue for URLs that need to be fixed with yt-dlp

## Usage

Create two services: one that is always running and another that is triggered by a periodic timer.

```sh

# Watch the mpd queue for changes
mpd-url watch

# Check the queue for any expired URLs and replace them
mpd-url update

```
