## zsh_universal

Attempt to create an opinionated, modular, & universal zshrc configuration for all Unix systems. Feel free to customize aliases, keybinds, functions, etc. Be sure to backup any previous zsh configuration files before installing.

### Installation

```sh
git clone https://github.com/minato-devv/zsh_universal.git && cd zsh_universal
mkdir -p ~/.config/zsh ~/.cache ~/.local/state
ln -s "$PWD/.zshenv" "$HOME/" && source "$HOME/.zshenv"
find "$PWD" -mindepth 1 -maxdepth 1 ! -name "README.md" ! -name "LICENSE" ! -name ".git" ! -name ".zshenv" -exec ln -s {} "$ZDOTDIR/" \;
```

Close the window or exit the session to ensure proper sourcing.
