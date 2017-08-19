## Introduction
============

The configuration file in this repo can be used to enable these features for your tmux macOS install (to install tmux refer to this page https://goo.gl/vmYTVQ):
1. Enable mouse scrolling 
2. Enable TPM (Tmux Plugin Manager) (https://github.com/tmux-plugins/tpm)
3. Enable the ThemePack plugin (https://github.com/jimeh)
4. Enable the Powerline Cyan theme 

Rename the tmux.conf file to .tmux.conf and copy it to your home directory "/.tmux.conf".

<img src="tmux_config_screenshot.gif" />

## Install TPM
=================
1. To install TPM, you need to clone TPM from github:

```
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

2. The configuration will use TPM to install the ThemePack plugin. Just make sure the path is same as in the command above



## Install Powerline Fonts
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

2. To enable the fonts in Iterm2 go to File -> Profiles -> Text and change font to one of the Powerline fonts. I use "13 Space Mono" as my default one in the screenshot above. For list of other fonts go to https://github.com/powerline/fonts

### Source/enable the tmux.conf file
================================
To enable/source the config file in tmux while running a session, type this in your tmux terminal

```
tmux source ~/.tmux.conf
```

This will run the plugins and you should see the new theme applied.
