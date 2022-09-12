# My personal vscode and zsh .dotfiles 💻

This repository contains my personal settings for VSCode and the zsh 👨‍💻.

## zsh setup

Install and setup the zsh. Comes preinstalled with OSX.

### Install [ohmyzsh](https://ohmyz.sh/)

Framework to manage the local zsh installation. Gives us the ability to easily install plugins and custom fonts.

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Install [Powerline Fonts](https://github.com/powerline/fonts)

```
git clone https://github.com/powerline/fonts.git --depth=1 &&
cd fonts &&
./install.sh &&
cd ..
```

### Install [PowerLevel10k](https://github.com/romkatv/powerlevel10k) zsh-theme

Follow the installation instructions [here](https://github.com/romkatv/powerlevel10k#getting-started).

## Add Plugins to zsh-installation

The following describes the installation of some zsh plugins.

### Syntax-Highlighting

Basic syntax highlighting in zsh.

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

### Basic Auto-Suggestion

Basic auto suggestions in zsh.

```
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

### Auto-Complete on 💪

Plugin that creates an index of frequently used folders. These can then be easily opened via `z FOLDER`.

```
git clone https://github.com/agkozak/zsh-z ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-z
```

### Check .zshrc

Your `.zshrc`should contain a plugins section. The installed plugins should be listed there like so:

```bash
#...
plugins=(
	git
	zsh-syntax-highlighting
	zsh-autosuggestions
	z
	brew
	macos
	extract
)
#...
```

## Git Config

Finally setup git.

```
git config --global user.name < USERNAME > &&
git config --global user.email < EMAIL > &&
git config --global --list
```

## Finale remarks

The full VSCode `settings.json` and full `.zshrc` can be found in the root of this git repository.
