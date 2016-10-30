# timur-i3-env
Refactored from my [i3-config](https://github.com/TimurKiyivinski/i3-config-desktop) to use a Powerline status bar instead.
It is a highly opinionated setup for my needs using my themes and liking.

Requires:
* [twmn](https://github.com/sboli/Twmn)
* [feh](https://github.com/derf/feh)
* [maim](https://github.com/naelstrof/maim)
* [playerctl](https://github.com/acrisci/playerctl)
* [imagemagick](https://github.com/ImageMagick/ImageMagick)
* [compton](https://github.com/chjj/compton)
* [rofi](https://davedavenport.github.io/rofi/)
* [lemonbar](https://github.com/LemonBoy/bar)
* [powerline](https://github.com/powerline/powerline)
* i3lock, i3-nagbar, URXVT

# setup
Copy `.Xresources` and `.config` to `~/`. You may have to modify the i3 screen setup as this is configured for dual monitors.
The `.config` directory includes my `i3` and `Powerline` config whereas `.Xresources` contains my `Rofi` and `URXVT` config.

# wallpaper setup
Wallpapers are selected on random from `~/.theme/wallpaper-*.png`. Example:
* wallpaper-0.png
* wallpaper-1.png
* wallpaper-2.png

# status bar setup
Create a file `status.py` as a symbolic link to powerline, eg. `/usr/lib/python3.5/site-packages/powerline/bindings/lemonbar/powerline-lemonbar.py`

# start-up programs
Add a list of programs as so into the `env` file.
```
executables=("nm-applet" "firefox" "spotify" "telegram" "owncloud" "redshift-gtk")
```

# screenshots
Desktop:
![desktop](screenshots/desktop.png)

# additional information
My shell uses [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) with the following config:
* [.zshrc](https://gist.github.com/TimurKiyivinski/5846fe2459544865ee11)
* [.zshenv](https://gist.github.com/TimurKiyivinski/4e69f98d20bc0e90ab70317b578a1e64)

## shortcuts
* `Super + D` Open Rofi
* `Super + Shift + S` Power Menu
* `Super + Shift + X` Lock Screen
* `Left Super + $N` switch to workspace `$N` on left monitor
* `Right Super + $N` switch to workspace `$N` on right monitor
