# rofi-lpass

Custom script for Rofi that allows you to copy passwords from your Lastpass vault.

## Features

* List all your entries
* Copy password of an entry
* Copy username / email of an entry
* Copy URL (if entry has an URL)
* Open URL (if entry has an URL)

## Installation

1. Make sure you have the requirements installed and available on your `PATH`:
   - [lastpass-cli](https://github.com/lastpass/lastpass-cli)
   - [xdg-utils](https://www.freedesktop.org/wiki/Software/xdg-utils/)
   - When using X11:
      - [xsel](http://www.vergenet.net/~conrad/software/xsel/)
      - either [xvkbd](http://t-sato.in.coocan.jp/xvkbd/) or [xdotool](https://www.semicomplete.com/projects/xdotool/)
   - When using Wayland:
      - [wl-clipboard](https://github.com/bugaevc/wl-clipboard)
      - [wtype](https://github.com/atx/wtype)
2. Symlink the script to somewhere on your `$PATH`: `ln -s $(pwd)/rofi-lpass ~/bin/rofi-lpass`.
3. Run rofi with this as a custom script: `rofi -modi lpass:rofi-lpass -show lpass`

## License

Copyright © 2017 Magnus Bergmark, 2019-2022 David H. Bronke. Code released under [the MIT license](LICENSE).
