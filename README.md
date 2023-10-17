# Qtile-config
My qtile config

To install:
* For Arch/Arch derivatives:
  * Install yay:
```
sudo pacmna -S base-devel
git clone https://aur.archlinux.org/yay.git && cd yay
makepkg -si
```

* Install the dependencies:

  * Debian based:

    ```
    sudo apt install lxsession picom copyq network-manager-applet pamac-tray-icon-plasma qtile i3lock-color rofi kitty nitrogen lxappearance qt5ct nerd-fonts xss-lock
    ```

    * Install [qtile-extras](https://github.com/elParaguayo/qtile-extras)
  
  * Arch based:

    ```
    yay -S lxsession picom copyq network-manager-applet pamac-tray-icon-plasma qtile qtile-extras i3lock-color rofi kitty nitrogen kitty lxappearance qt5ct nerd-fonts xss-lock
    ```
  * [Rofi power menu](https://github.com/jluttine/rofi-power-menu)


Clone the repo:

```
git clone https://github.com/DNM1008/Qtile-config.git && cd Qtile-config
```

Copy everything to the config directory:

```
cp -r qtile ~/.config/
```
You can edit and the config file at `~/.config/qtile/config.py`.
Autostart programs and external tray icons (copyq, nm-applet, blueman, picom, pamac-tray-icon) are at `~/.config/qtile/autostart.sh`.

By defaults:
* Super + Q closes the focused window
* Super + R launches a run prompt, but I only use it when other keybinds don't work
* Super + W launches Firefox if installed
* Super + Enter launches Kitty if installed
* Super + D launches Discord if installed
* Super + M launches Thunderbird if installed
* Super + C launches VSCode if installed 
* Super + V launches CopyQ main window
* Super + P launches Rofi
* Super + Shift + S launches flameshot if installed, I set the default to just copy the screen shot to the clipboard instead of to a file
* Super + T toggles floating
  * Super + LMB moves the window
  * Super + RMB resizes the window
* Super + F toggles fullscreen
* Super + Shift + P launches Rofi Power Menu
* Super + Minus shrinks the window horizontally
* Super + Equal expands the window horizontally
* Super + H/J/K/L moves the focus onto window of relative position
* Super + Shift + H/J/K/L moves the focused window in the stack or between the columns
* Super + Tab cycles between layouts
* There are other keybindings for layouts that I don't use (yet) but decided to leave them as is if you can make use of them

The programs listed are the ones I use and recommends, but if you don't want to use them, simply install the ones you like and change the config file, though you might want to install kitty first, just so it's easier to change the config.
  

You might want to install xmodmap and/or input-remapper to edit your keyboard mappings.

You might have to make the autostart file executable: `sudo chmod +x ~/.config/qtile/autostart.sh`

For my other configs, you should check out [this](https://github.com/DNM1008/Other-configs)

Special thanks to [DT](https://gitlab.com/dwt1), this config file is just his config file but customised a little bit by me.
[His YouTube Channel](https://www.youtube.com/@DistroTube)

You can take a look at the config file for the keybindings
