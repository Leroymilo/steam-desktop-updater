# Steam desktop files updater
This script creates desktop entries for Steam games

## Dependencies

This program requires a few dependencies to work.
To install them locally, run:

```bash
python3 -m pip install --user pillow vdf steam
```

## Usage

The script works by passing the steam root path, as:
```
./steam_desktop_updater.py <dir-path>
```
The default path would be:
```
./steam_desktop_updater.py  ~/.local/share/Steam
```
For Steam flatpack users the path would be:
```
./steam_desktop_updater.py ~/.var/app/com.valvesoftware.Steam/data/Steam
```

Added a new option `-g` or `--games`, it will allow you to choose which games will have a shortcut created.</br>
To use, add `-g <game_id>` at the end of the command. You can submit multiple ids as comma separated entries : `-g "<game_id1>, <game_id2>, <game_id3>, ..."`.</br>
You can find the id of a game by checking its store page (it's in the url).