# Dotfiles

## zsh

### ohmyzsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"


### Install Powerline Fonts
```
git clone https://github.com/powerline/fonts.git --depth=1 &&
cd fonts &&
./install.sh &&
cd ..
```

### Theme
https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k

### Plugins
Syntax-Highlighting
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
### Auto-Suggestion
```
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

## Git Config
```
git config --global user.name < USERNAME > &&
git config --global user.email < EMAIL > &&
git config --global --list
```
