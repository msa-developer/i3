# i3

![i3](./i3Window.png)

### For Disabling Screen Tearing For amdgpu only `/etc/X11/xorg.conf.d/20-amdgpu.conf `

```
Section "Device"
    Identifier "AMD Graphics"
    Driver "amdgpu"
    Option "TearFree" "true"
EndSection
```

### For Making The Working of touchpad in laptop properly in i3 wm `/etc/X11/xorg.conf.d/90-touchpad.conf`

```
Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
    Option "NaturalScrolling" "true"
    Option "TappingButtonMap" "lmr"
    Option "ScrollMethod" "twofinger"
    Option "ClickMethod" "clickfinger"
EndSection

```
