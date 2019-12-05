# dots files

### Install fonts

[Fontawesome](http://fontawesome.io/) | [cheatsheet](http://fontawesome.io/cheatsheet/)

### i3

Dependencies:

- i3-gaps
- i3blocks
- playerctl
- zsh
- oh-my-zsh
- terminator
- arandr
- feh
- compton

### Enable touchpad

```
# https://cravencode.com/post/essentials/enable-tap-to-click-in-i3wm/
sudo mkdir -p /etc/X11/xorg.conf.d && sudo tee <<'EOF' /etc/X11/xorg.conf.d/90-touchpad.conf 1> /dev/null
Section "InputClass"
        Identifier "touchpad"
        MatchIsTouchpad "on"
        Driver "libinput"
        Option "Tapping" "on"
        Option "NaturalScrolling" "on"
        Option "ScrollMethod" "twofinger"
EndSection

EOF
```

### TODO

- Switching display modes
