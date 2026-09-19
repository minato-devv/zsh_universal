## zsh_universal

Attempt to create an opinionated, modular, & universal zshrc configuration for all Unix systems. Feel free to customize aliases, keybinds, functions, etc.

### Installation

```sh
git clone https://github.com/minato-devv/zsh_universal.git && cd zsh_universal
mkdir -p ~/.config/zsh
ln -s "$PWD/.zshenv" "$HOME/" && source "$HOME/.zshenv"
find -type f ! -name ".zshenv" -mindepth 1 -maxdepth 1 -exec ln -s "$PWD/{}" "$ZDOTDIR/" \;
```

Close the window or exit the session to ensure proper sourcing.
