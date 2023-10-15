# Qtile-config
My qtile config

To install:

Install the dependencies:

Debian based:

```
sudo apt install lxsession picom copyq network-manager-applet pamac-tray-icon-plasma qtile qtile-extras i3lock-color rofi flameshot firefox thunderbird pcmanfm konsole
```

Arch based:

```
yay -S lxsession picom copyq network-manager-applet pamac-tray-icon-plasma qtile qtile-extras i3lock-color rofi flameshot firefox thunderbird pcmanfm konsole
```

Clone the repo:

```
git clone https://github.com/DNM1008/Qtile-config.git && cd Qtile-config
```

Copy everything to the config directory:

```
cp -r qtile ~/.config/
```
You can edit and the config file at `~/.config/qtile/config.py`.
Autostart programs and external tray icons (copyq, nm-applet, blueman, picom, pama-tray-icon) is at `~/.config/qtile/autostart.sh`.

You might want to install xmodmap and/or input-remapper to edit your keyboard mappings.

Special thanks to [DT](https://gitlab.com/dwt1), this config file is just his config file but customised a little bit by me.
