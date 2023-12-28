# Initial setup of working environment


## From Console
1. Install brew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
2. Install iterm2
```bash
brew install --cask iterm2
```

3. Install Rectangle (screen management)
```bash
brew install --cask rectangle
```

4. Install Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

5. Install Powerlevel10k
```bash
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

Then open ~/.zshrc file with `vim ~/.zshrc` and set `ZSH_TEME=“powerlevel10k/powerlevel10k”`

<img src="img/zsh_theme.png" width="500px">

6. Quit iTerm and reopen. 

Go thought the configurator that will pop up on the console according to your needs

7. iTerm2 customizations

iTerm → Settings → Profiles → Colors → Color Presets → Solarized Dark

8. Word jumps and delete

iTerm → Settings → Profiles → Keys
- Left option → Esc+
- add a new key mapping: Key Mapping tab → Press `+` → Press `⌥` + `←` → Select “Send Escape Sequence” for action. → Input `b` on Esc+.
- add a new key mapping: Key Mapping tab → Press `+` → Press `⌥` + `→` → Select “Send Escape Sequence” for action. → Input `f` on Esc+.

<img src="img/escaping.png" width="500px">
<img src="img/move_forward.png" width="500px">
<img src="img/removing_jump.png" width="500px">


9. Auto-suggestions plugin
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

to set the plugin, run `vim ~/.zshrc` and set `plugins=(git zsh-autosuggestions)`
<img src="img/zsh_suggestions.png" width="500px">

10. Remove apple sign

Open `~/.p10k.zsh` → Comment out `os_icon`

<img src="img/remove_apple_sign.png" width="500px">

10. AWS CLI
```bash
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
sudo installer -pkg AWSCLIV2.pkg -target /
```

11. AWS Session manager plugin
```bash
curl "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/sessionmanager-bundle.zip" -o "sessionmanager-bundle.zip"
unzip sessionmanager-bundle.zip
sudo ./sessionmanager-bundle/install -i /usr/local/sessionmanagerplugin -b /usr/local/bin/session-manager-plugin
```

12. SdkMan
```bash
curl -s "https://get.sdkman.io" | bash
source "$HOME/.sdkman/bin/sdkman-init.sh"
sdk version
sdk install java
```

13. Docker
```bash
brew install --cask docker
```

14. Docker
```bash
brew install --cask postman
```

15. VS Code
```bash
brew install --cask visual-studio-code
```

16. IntellijIdea
```bash
brew install --cask intellij-idea
```

17. Change default scrolling direction

Click apple menu (left top corner) → System Preferences → click Scroll & Zoom → toggle Natural scroll direction to off

18. Microsoft Teams
```
brew install --cask microsoft-teams
brew install --cask microsoft-outlook
```

19. Microsoft Outlook
```
brew install --cask microsoft-outlook
```

Open Project ->  Choose location of umbrella directory  
