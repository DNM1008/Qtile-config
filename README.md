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
 * Debbian based: Take a look at the programs in the list of programs for Arch, I you will need to install them, there might be hoops to jump through that I don't know how, particularly `qtile-extras`
  
  * Arch based:

    ```
    yay -S lxsession picom copyq network-manager-applet qtile qtile-extras i3lock-color rofi alacritty nitrogen kitty lxappearance qt5ct nerd-fonts xss-lock maim xclip xwallpaper fortune-mod
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

By defaults, provided that these applications are installed:
* Super + D launches Discord
* Super + E launches PCManFM
* Super + Enter launches Alacritty
* Super + F toggles fullscreen
* Super + M launches Mailspring
* Super + P launches Rofi
* Super + Q closes the focused window
* Super + R launches a run prompt, but I only use it when other keybinds don't work
* Super + T toggles floating
  * Super + LMB moves the window
  * Super + RMB resizes the window
* Super + V toggles CopyQ main window
* Super + W launches Firefox if installed
* Super + Shift + S set up screenshot region, I set the default to just copy the screenshot to the clipboard instead of to a file
  * Alt + Shift + S takes a screenshot of the whole desktop and save it to ~/.cache/screenshot.png because the main screenshot short is wonky when taking the region the size of the screen 
* Super + Shift + P launches Rofi Power Menu
* Super + Minus shrinks the window horizontally
* Super + Equal expands the window horizontally
* Super + H/J/K/L moves the focus onto window of relative positions
* Super + Shift + H/J/K/L moves the focused window in the stack or between the columns
* Super + Tab cycles between layouts
* There are other keybindings for layouts that I don't use (yet) but decided to leave them as is if you can make use of them

For funsies, you can click on the arch glyph on the top left (the first widget on the bar) and you should have a dunst notification that quotes a quote from fortune

The programs listed are the ones I use and recommends, but if you don't want to use them, simply install the ones you like and change the config file, though you might want to install kitty first, just so it's easier to change the config.
  

You might want to install xmodmap and/or input-remapper to edit your keyboard mappings.

You might have to make the autostart file executable: `sudo chmod +x ~/.config/qtile/autostart.sh`

For my other configs, you should check out [this](https://github.com/DNM1008/Other-configs)

Special thanks to [DT](https://gitlab.com/dwt1), this config file is just his config file but customised a little bit by me.
[His YouTube Channel](https://www.youtube.com/@DistroTube)

You can take a look at the config file for the keybindings
