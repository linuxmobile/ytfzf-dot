# ytfzf-dot
My Own config for ytfzf-dot

```sh
git clone https://github.com/linuxmobile/ytfzf-dot &&
cd ~/ytfzf-dot &&
rsync -avxHAXP --exclude '.git*' .* ~/ 
```

```sh
echo -n "export YTFZF_EXTMENU='rofi -dmenu -fuzzy -width 1000'" >> ~/.zshrc &&
echo -n "export YTFZF_ENABLE_FZF_DEFUALT_OPTS=0" >> ~/.zshrc &&
echo -n 'export alias yt="~/.scripts/yt-r"'
```

