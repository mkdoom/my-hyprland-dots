(please dont mind the commits)
**hyprlock by narukami3737 on discord**

# My hyprland dots!!!

Heya bud! if you are here, it seems you liked how my hyprland looks!
Anyways... if you need something, here's the thing.

## Screenshot!
![How's my rice?](screenshot.png)

# Dependencies!
- **WM**: [Hyprland](https://github.com/hyprwm/Hyprland) - A dynamic tiling Wayland compositor.
- **Compositor**: Wayland for smooth and modern graphics.
- **Terminal Emulator**: [Kitty](https://github.com/kovidgoyal/kitty) -  If you live in the terminal, kitty is made for you! Cross-platform, fast, feature-rich, GPU based.
- **App launcher**: [Wofi](https://github.com/SimplyCEO/wofi) - Wofi is a launcher/menu program for wlroots based wayland compositors such as sway. 
- **Status bar and stuff**: [Waybar](https://github.com/Alexays/Waybar) - A highly customizable status bar.
- **Notifications**: [Mako](https://github.com/emersion/mako) - A lightweight Wayland notification daemon.
- **Color Scheme Generator**: [Pywal16](https://github.com/eylles/pywal16) - Generates 16 colors from your wallpaper.

## What do i will give you?
- My hyprland config folder (hypr).
- Waybar config.
- Fastetch (already has some images and gifs), just make sure to make reference them.
- Kitty configs.
- Wofi configs.
- Wallpapers.

And before you ask, no. I will **NOT** help you change the timezone on waybar. Please do yourself (modules.jsonc, search for line 114).

# HOW TO INSTALL

Maybe you're asking youself... "how do i install it? im too lazy to manual-do this..." dont worry but! i gotchu
1. Clone this repository.
```bash
git clone https://github.com/mkdoom/my-hyprland-dots
cd my-hyprland-dots
```
if u dont have git (you should, but if u dont)...
```
sudo pacman -S git
```

2. Install dependencies...

```bash
sudo pacman -S hyprland kitty wofi waybar mako zsh ttf-jetbrains-mono ttf-jetbrains-mono-nerd hyprpaper
yay -S python-pywal16
```

(PS: if u dont have [yay](https://github.com/Jguer/yay?tab=readme-ov-file)...)
 
 ```
sudo pacman -S --needed git base-devel
git clone https://aur.archlinux.org/yay-bin.git
cd yay-bin
makepkg -si
```

(You will install through the binary here, it's more easy AND ur cpu will be alot more happy with this one...)

3. Copy the configs to your .config dir.
```bash
cp -r .config/* ~/.config/
```

4. PLEASE PLEASE PLEASE DO THIS

 **IMPORTANT**: If you want your colors to sync with pywal (like, the rice goes around it) please change in waybar (if you will use it) and wofi configs where source is referencing my user...

5. Just restart.
```bash
reboot
```

# Notes...

Waybar is NOT set at start, also is big asf...

Anyways, if you want it to start when your hyprland, add this to hyprland.conf

```
exec-once = waybar
```
