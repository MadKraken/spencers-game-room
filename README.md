# Spencer's Game Room

Pick a platform and watch speedruns on the TV in Spencer's gaming room. For a random game and
category on that platform, the site plays the best-placed run that has a YouTube or Twitch video,
then rolls the next one when it ends.

Live site: https://madkraken.github.io/spencers-game-room/

Run data comes from the [speedrun.com API](https://github.com/speedruncomorg/api). ROM hacks, mods
and fan games are skipped unless you turn them on in Settings.

Spencer's button sounds (off by default, in Settings) are
["Gaming Controller Playing Sounds 1"](https://freesound.org/people/Joao_Janz/sounds/477534/) by
Joao_Janz on Freesound, released under CC0. It's converted to a mono MP3 in `controller.mp3`.

## Running it locally

```bash
python serve.py
```

Then open http://localhost:8765. YouTube and Twitch won't play embeds from a page opened straight
from disk, so it needs to be served.
