# ytfzf-dot

### 🎀 My Settings and Scripts to get YTFZF working awesome.

_special thanks to [ytfzfim](https://github.com/thatonecalculator/ytfzfim) for this amazing tool_

## 🔮 Clone and Sync repo

```sh
git clone https://github.com/linuxmobile/ytfzf-dot &&
cd ~/ytfzf-dot &&
rsync -avxHAXP --exclude '.git*' .* ~/ 
```

## 📌 Add rofi and an alias to your shell (i'm using zsh as example)

```sh
echo -n "export YTFZF_EXTMENU='rofi -dmenu -fuzzy -width 1000'" >> ~/.zshrc &&
echo -n "export YTFZF_ENABLE_FZF_DEFUALT_OPTS=0" >> ~/.zshrc &&
echo -n 'export alias yt="~/.scripts/yt-r"'
```

## 🛠️ Add beautiful Keybind to your WM.

_ This example is only for DWM _

```sh
/* YTFZF scripts. Run script and quit killing mpv */
{MODKEY, XK_y, spawn, SHCMD("~/.scripts/yt-r")},
{MODKEY|ShiftMask, XK_y ,spawn, SHCMD("pkill -9 mpv")},
```
