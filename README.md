# NOTE! I HAVE MOVED to new ARCH-HYPRLAND install script REPO as part of my install script clean up
- [`Link`](https://github.com/JaKooLit/Arch-Hyprland)

### A re-structured install script of my Hyprland-v3 [`Link`](https://github.com/JaKooLit/Hyprland-v3)

![alt text](https://github.com/JaKooLit/Ja-Hyprland/blob/main/screenshots/Sample-Tokyo-waybar.png "Default")

![alt text](https://github.com/JaKooLit/Ja-Hyprland/blob/main/screenshots/dual-panel-light-dark-switch.png "Default")

### 📷 you can find more screenshots in the screenshots directory

### 📽️ youtube video showcase: [`Youtube Link`](https://youtu.be/otda1nXJ5Dg?si=Wbb8eg-u3Y-tDnDQ)



### ✨ A video walk through my dotfiles[`Link`](https://youtu.be/fO-RBHvVEcc?si=ijqxxnq_DLiyO8xb)


### 🆕  What's new compared to my V3
- restructured Install script
- Can modify the packages easily. (install-scripts/00-hypr-pkgs.sh) edit as desired
- Added Tokyo-night-theme and TokyoNight-SE icons
- using dunst instead of mako
- Added Tokyo-Night SDDM Theme 
- Use a wofi-power menu instead of wlogout
- Added the following: 
   - a. gnome-system-monitor
   - right click on cpu waybar module
   - b. nvtop - right click on temperature waybar module


### 👀 NVidia GPU Owners.
- By default, nvidia-dkms will be installed. and only supports GTX 900 and newer. If required to install older driver, edit the nvidia.sh in scripts-folder


### ✨ to run
> clone this repo by using git. Change directory, make executable and run the script
```bash
git clone https://github.com/JaKooLit/Hyprland-v4.git
cd Hyprland-v4
chmod +x install-v4.sh
./install-v4.sh
```
### ✨ for ZSH and OH-MY-ZSH installation
> do this once installed and script completed; do the following to change the default shell zsh
```bash
chsh -s $(which zsh)
zsh
source ~/.zshrc
```
- reboot or logout
- by default gnzh theme is installed. You can find more themes from this [`OH-MY-ZSH-THEMES`](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)
- to change the theme, edit ~/.zshrc ZSH_THEME="desired theme"

### 📒 Notes
- super h for launching a small help file
- super e to view / edit settings, monitor, keybinds, Environment Variables, etc
- go through the keybinds. There are alot of hidden features like dual panel, change waybar styles, change wallpaper, etc... its too long to put all in the readme!!!

### 🛣️ Roadmap:
- [ ] Install zsh and oh-my-zsh without necessary steps above
- [ ] possibly adding gruvbox themes, cursors, icons
- [ ] adding vertical waybar 
- [X] ~~Use kitty in favor of foot~~ - Dropped the idea of kitty. Kitty is using twice memory compared to foot.

### ⚠️ some known issues
- reports from members of my discord, states that some users of nvidia are getting stuck on sddm login. credit  to @Kenni Fix stated was 
```  
 while in sddm press ctrl+alt+F2 or F3
log into your account
`lspci -nn`, find the id of your nvidia card
`ls /dev/dri/by-path` find the matching id
`ls -l /dev/dri/by-path` to check where the symlink points to 
)
7. add "env = WLR_DRM_DEVICES,/dev/dri/cardX" to the ENVvariables config (.config/hypr/configs/ENVariables.conf)  ; X being where the symlink of the gpu points to
```
- more info from the hyprland wiki [`Hyprland Wiki Link`](https://wiki.hyprland.org/FAQ/#my-external-monitor-is-blank--doesnt-render--receives-no-signal-laptop)


### 👍👍👍 Thanks and Credits!
- shout out to CooSee from Gentoo forums for the nice rainbow borders


## 💖 Support
- a Star on my Github repos would be nice 🌟

- Subscribe to my Youtube Channel [YouTube](https://www.youtube.com/@Ja.KooLit) 

- You can also buy me Coffee Through ko-fi.com 🤩

<a href='https://ko-fi.com/jakoolit' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />


