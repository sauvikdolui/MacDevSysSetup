# MacDevSysSetup
Useful setups commands for a new Mac

### Userful terminal commands for Mac

#### 1. Xcode command line tool installation
`xcode-select --install`

#### 2. Show hidden files on Finder
`defaults write com.apple.finder AppleShowAllFiles YES && killall Finder`

#### 3. Homebrew installation
`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

#### 4. Cocoapods installation
`gem install -n /usr/local/bin cocoapods`

### 5. Installtion of the Oh My ZSH Terminal with Custom Theme `agnoster`

1. Install ZSH with `sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
2. Clone  https://github.com/powerline/fonts, make `install.sh` executable by `chmod +x install.sh`. Run it to install fonts.
3. Open `.zshrc` to chage the theme as `vim ~/.oh-my-zsh/.zshrc`
4. Move to line no 11 to change the theme line no. 11 `ZSH_THEME="agnoster"`
5. Import custom theme [`Homebrew Custom.terminal`](https://raw.githubusercontent.com/sauvikdolui/MacDevSysSetup/master/resources/Homebrew%20Custom.terminal) and make it as default one.
6. Set font Roboto Powersheel from Preference **CMD + ,**

### 6. Disable Screenshot Shadows
`defaults write com.apple.screencapture disable-shadow -bool TRUE && killall SystemUIServer`

### 7. Mojave Bootable USB Creation
sudo ~/Documents/Softwares/Install\ macOS\ Mojave.app/Contents/Resources/createinstallmedia --volume /Volumes/SAUVIK-SAND --nointeraction && say Mojave Drive Created 
