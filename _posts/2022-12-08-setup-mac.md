---
title: setup mac
date: 2022-12-08 16:50:00 -500
categories: [mac, software]
tags: [laptops,macbook,homebrew,initial]
---
# setup mac

Page to setup my mac in the event of the worst happens :) 

## Install Homebrew

First things first, install homebrew. 

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Install apps via homebrew

```bash
brew install azure-cli git pyenv pyenv-virtualenv python @3.10 terraform sqlite xz
```

```bash
brew install --cask google-chrome dbeaver-community adobe-acrobat-reader iterm2 microsoft-azure-storage-explorer microsoft-edge onedrive powershell the-unarchiver visual-studio-code warp whatshapp discord
```

## Terminal changes

- Use fingerprint as sudo


    open /etc/pam.d/sudo file as sudo user    
    ```bash
    sudo code /etc/pam.d/sudo
    ```
    
    now add the following line at the start of the file:
    ```bash
    auth sufficient pam_tid.so
    ```

