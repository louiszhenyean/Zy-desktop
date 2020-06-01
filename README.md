# Zyubuntu
Setup for my Ubuntu Desktop, install and uninstall some applications that I always use and never use.  
Also some configurations for the Desktop, Icons and keyboard shortcut.  

# Prerequisite
Install all the requirements and tools  
```
sudo apt install git curl chrome-gnome-shell gnome-tweak-tool 
       \ fonts-powerline fonts-noto-color-emoji 
       \ tree neofetch zsh tmux tilix python-nautilus nmap
````

Clone the repository
```
git clone https://github.com/louiszhenyean/Zyubuntu.git
git clone https://github.com/louiszhenyean/hackthebox /home/zyaire/Desktop/hackthebox
```

Copy the files and make activate the configurations
```
mkdir /home/zyaire/Desktop/git
mkdir /home/zyaire/Desktop/git/MyProject
ln -s /home/zyaire/Desktop/git ~/git
ln -s /home/zyaire/Desktop/hackthebox ~/hackthebox  
cp hardcoding.jpg /usr/share/backgrounds/
gsettings set org.cinnamon.desktop.background picture-uri "/usr/share/backgrounds/hardcoding.jpg"
cp tmux.conf ~/.tmux.conf
cp ~bashrc ~/.bashrc.bck
cp bashrcKali2019 ~/.bashrc
source .bashrc
tmux source-file .tmux.conf
```

# Click this to install Nerd-Fonts (Terminal Emoji)
https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete.ttf

# Self changing setting
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

`git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k`

`cp zshrc ~/.zshrc`

`chsh -s $(which zsh)`

`sudo update-alternatives --config x-terminal-emulator`

For OCD, can replace the Tilix to the default Terminal icon  
`/usr/share/icons/hicolor/scalable/apps/com.gexperts.Tilix.svg`

# Personal Shortcuts
Always use easy shortcuts, lol
```
sudo cp /bin/xdg-open /bin/open
sudo ln -s /bin/bash /bin/b
sudo ln -s /bin/zsh /bin/z 
```

# Install SearchSploit
`sudo git clone https://github.com/offensive-security/exploitdb.git /opt/exploitdb`

`sed 's|path_array+=(.*)|path_array+=("/opt/exploitdb")|g' /opt/exploitdb/.searchsploit_rc > ~/.searchsploit_rc`

`sudo ln -sf /opt/exploitdb/searchsploit /usr/local/bin/searchsploit`


# Install Gnome Extensions
https://extensions.gnome.org/extension/19/user-themes/

https://extensions.gnome.org/extension/307/dash-to-dock/
