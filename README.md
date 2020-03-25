#### CaptainEureka's personal config files
---
This is a collection of my personal configuration files.
I'm currently using Manjaro with `i3-gaps-rounded` and KDE/Plasma (until I properly configure multi-monitor support in `i3`.)

Some details about my setup:

- **WM**: [i3-gaps-rounded](https://github.com/resloved/i3/) ([AUR](https://aur.archlinux.org/packages/i3-gaps-rounded-git/))
- **DE**: [KDE/Plasma](https://kde.org/plasma-desktop)
- **Compositor**: [picom]() (with `dual-kawase` blur)
- **OS**: Manjaro
- **Shell**: [zsh](https://wiki.archlinux.org/index.php/Zsh)
  - Using: [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh) with the [pi](https://github.com/tobyjamesthomas/pi) theme
- **Terminal Emulator**: [kitty](https://github.com/kovidgoyal/kitty/) / `Konsole`
- **Editor**: [Neovim](https://github.com/neovim/neovim/)
- **File Manager**: [nnn](https://github.com/jarun/nnn/) / [thunar](https://git.xfce.org/xfce/thunar/)
- **Launcher/run**: [rofi](https://github.com/davatorium/rofi)
- **Bar**: [polybar](https://github.com/polybar/polybar)
- **Browser**: Firefox (with my personal [userChrome.css](https://github.com/CaptainEureka/))

---

##### Notable features
---

- Rofi menus: scrot, power, web-search, wifi, appmenu (fullscreen), applist, wallpaper-switcher

##### Screenshots
---

*Some scrots*

##### Fonts
---

##### Keybinds
---

##### To-Do:
---
- [x] Implement **u/adi1090x** Rofi dummy window for background blur effect.
- [ ] Implement theme-switcher
  - [ ] Input should be YAML/JSON
  - [ ] Should use `Jinja2` engine or just use `Pywal`? -> decided to just use 'pywal' for templating (might try out 'wpg')
- [ ] Refactor `rofi` and `polybar` configs to get rid of duplicated code
      eg. `rofi` configs contain `theme.rasi` files which themselves contain much that can be placed in a 
          `base.rasi` file which unifies all. Making the `-no-config` flag in most `rofi` scripts unnecessary.
      eg. for `polybar` would like a more elegant solution for handling bars over multiple wms.
