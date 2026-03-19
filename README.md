# Kanade Cursors~
The unofficial linux port of **Yoisaki Kanade from Nightcord at 25:00's cursors**, mainly known from a rhythm game **"HATSUNE MIKU : COLORFUL STAGE!"**.

## Notes
Currently **only hyprcursor is supported** as I have not found a way to make it into XCursor. But XCursor might find it's way here in the future.

And also...

- Sizes 32 and above are supported for hyprcursor. Anything below would just crop the cursor!
- Sizes 32 and 64 are only supported for xcursor.

## Installation

### Any distros using Hyprland :
1. Grab the latest cursor release file [from here](https://github.com/PixieXD/KanadeCursors/releases).
2. Extract the tar ball.
3. Copy / Move the contents of the folder to either `~/.local/share/icons` or `~/.icons`. 
4. Set the icon theme by either setting up the Env variables or utilising `hyprctl` :

```json
# Env Variables (using hyprcursor)
env = HYPRCURSOR_THEME,KanadeCursors
env = HYPRCURSOR_SIZE,32

# hyprctl setcursor
hyprctl setcursor KanadeCursors 32
```
Note that Hyprland must be restarted by running `hyprctl dispatch exit` for the icons to take effect.

### Other DEs
1. Grab the latest cursor release file [from here](https://github.com/PixieXD/KanadeCursors/releases).
2. Extract the tar ball.
3. Copy / Move the contents of the folder to either `~/.local/share/icons` or `~/.icons`. 
4. Set the icon theme by setting up the Env variables :

```json
# Env Variables
env = XCURSOR_THEME,KanadeCursors
env = XCURSOR_SIZE,32
```
Restart and your cursor *should* be ready to go. If not, refer to your local DE manual for cursor theming.

## Credits!!

### Kanade cursors for windows :
- BLZ (Twitter : BLZ_pixel) : **Making this and the other unit's cursors <3** \
- Original Tweet : https://x.com/colorfulstageen/status/1984410152657723616?s=46 \
- Source : https://colorfulstage.com/media/download/ \

### Tools : 
- [`win2*`](https://github.com/quantum5/win2xcur) for making conversions from window cursors to xcursor possible.
- [`hyprcursor-utils`](https://github.com/hyprwm/hyprcursor) for the conversion of xcursor to hyprcursor.