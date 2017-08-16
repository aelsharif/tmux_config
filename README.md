## Introduction
============

This config file can be used to enable these features in your tmux file.
1. Enable mouse scrolling 
2. Enalbe TPM (Tmux Plugin Manager) (https://github.com/tmux-plugins/tpm)
3. Enalbe the ThemePack plugin (https://github.com/jimeh)
4. Enable the Powerline Cyan theme 

Copy this file to your home directory "/". Your file should be in "/.tmux.conf"

<img src="tmux_config_screenshot.gif" />

## Installing TPM
=================
1. To install TPM, all you need is to clone TPM from github:

```
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

2. The config file will use that file to install plugin. Just make sure the path is same as in the command above



## install Powerline fonts
==============================
The ThemePack plugin uses powerline fonts. If you don't have those fonts installed the theme wouldn't look right. To install the fonts follow these steps:

1. run these lines of code:

```
 # clone
git clone https://github.com/powerline/fonts.git
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts
```

2.  If Iterm2 go to File -> Profiles -> Text and change font to one of the Powerline fonts. I use "13 Space Mono" as my default one. For list of files go to https://github.com/powerline/fonts

### Source the tmux.conf file
================================
To enable/source the config file in tmux while running a session, type this in your tmux terminal

```
tmux source ~/.tmux.conf
```

This will run the plugins and you should see the new theme.
