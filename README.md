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
`sudo gem install -n /usr/local/bin cocoapods`

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
```
sudo ~/Documents/Softwares/Install\ macOS\ Mojave.app/Contents/Resources/createinstallmedia --volume /Volumes/SAUVIK-SAND --nointeraction && say Mojave Drive Created 
```

### Xcode Customization
* `defaults write com.apple.dt.Xcode ShowBuildOperationDuration -bool YES`
* Search in AppStore and install `Dev Cleaner for Xcode`
* Toolchain: Install latest version of Swift compilers from https://www.swift.org/download/. For an old version of Swift Compiler try installing https://download.swift.org/swift-5.3.2-release/xcode/swift-5.3.2-RELEASE/swift-5.3.2-RELEASE-osx.pkg. You may need to change the version based on the one you are looking for.

### Slack:
https://slack.com/intl/en-in/downloads/mac

### Microsoft Teams:
https://www.microsoft.com/en-in/microsoft-teams/download-app

### Sublime Text:
Download https://www.sublimetext.com/3
#### Install JSON Prettyfier: 
```
cd /Applications/Sublime\ Text.app/Contents/MacOS/Packages 
git clone https://github.com/dzhibas/SublimePrettyJson.git "Pretty JSON"
cd Pretty\ JSON/
git checkout st3
```
Use `⌘` + `^` + `J` to prettify. More at [Pretty JSON Package Read Me](https://packagecontrol.io/packages/Pretty%20JSON)

https://opensource.apple.com/source/xnu/xnu-792.2.4/libkern/libkern/sysctl.h.auto.html
