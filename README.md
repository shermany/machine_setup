# machine setup repo

Setup notes, dotfiles, etc...

## Apps and Utilities

### Chrome
### Dropbox
### 1password
### homebrew
### git (brew)

#### Enable colors

https://nathanhoad.net/how-to-colours-in-git

#### Setup your name/email

```
git config --global user.email "sean.hermany@gmail.com"
git config --global user.name "Sean Hermany"
```

#### Squelch the annoying message about the git push behavior change (old news)

```
git config --global push.default simple
```

### ack (brew)
### tree (brew)
### wget (brew)
### Caffeine (app store)
### Sublime Text 3
### iTerm2

1. Load latest sunbleh colors from this repo (thanks emery.)
2. Set terminal type to xterm (don't use 256 color mode)
3. Set left/right option keys to report as +Esc

### emacs (see emacs folder in this repo)

### pygmentize (for ccat alias)
(after updating to latest 2.7 series python)
```
$ pip install Pygments
```
### Adium
### Evernote

-----------------------------------------------------------------------

## Config

### .bashrc and .bash_profile

Contents of .bash_profile:

```
# Set architecture flags
export ARCHFLAGS="-arch x86_64"
# Ensure user-installed binaries take precedence
export PATH=/usr/local/bin:$PATH
# Load .bashrc if it exists
test -f ~/.bashrc && source ~/.bashrc
```

### emacs.d and .emacs file

### Remap capslock key to Ctrl in Settings

### Turn off "natural" scroll

### Rename computer

```
sudo scutil --set HostName [NewHostNameHere]
```

### Show the Library folder in finder:

```
chflags nohidden ~/Library/
```

### Make OSX Dock display faster

```
defaults write com.apple.Dock autohide-delay -float 0
defaults write com.apple.dock autohide-time-modifier -float 0.15
killall Dock
```

#### To Undo:

```
defaults delete com.apple.Dock autohide-delay
defaults delete com.apple.dock autohide-time-modifier
killall Dock
```

-----------------------------------------------------------------------

## Languages/Runtimes

* Python latest 2.7 (install on OSX via .pkg from python.org)
* nvm/node
* Java
* Clojure
* Scala

