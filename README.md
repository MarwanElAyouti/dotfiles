# Dotfiles

My personal configuration files for Unix-based systems.

## Contents

- **`.zshrc`** - Zsh shell configuration
- **`.tmux.conf`** - tmux terminal multiplexer configuration

## Installation

### Prerequisites

Install GNU Stow via your package manager:

```bash
# Ubuntu/Debian
sudo apt install stow

# macOS
brew install stow

# Arch Linux
sudo pacman -S stow

# Fedora
sudo dnf install stow
```

### Setup

1. Clone the repository to your home directory:

```bash
git clone https://github.com/MarwanElAyouti/dotfiles.git ~/dotfiles
```

2. Navigate to the dotfiles directory:

```bash
cd ~/dotfiles
```

3. Use GNU Stow to create symlinks:

```bash
stow .
```

This will automatically create symlinks in your home directory for all configuration files.

### Uninstalling

To remove the symlinks:

```bash
cd ~/dotfiles
stow -D .
```

## Requirements

- **GNU Stow** - Symlink farm manager
- **Zsh** - Install via your package manager (`apt`, `brew`, `pacman`, etc.)
- **tmux** - Install via your package manager

### Recommended Utilities

These configurations work best with the following modern command-line tools:

```bash
# Ubuntu/Debian
sudo apt install zoxide ripgrep fd-find fzf

# macOS
brew install zoxide ripgrep fd fzf

# Arch Linux
sudo pacman -S zoxide ripgrep fd fzf

# Fedora
sudo dnf install zoxide ripgrep fd-find fzf
```

- **[zoxide](https://github.com/ajeetdsouza/zoxide)** - Smarter cd command that learns your habits
- **[ripgrep (rg)](https://github.com/BurntSushi/ripgrep)** - Faster alternative to grep
- **[fd](https://github.com/sharkdp/fd)** - Faster and more user-friendly alternative to find
- **[fzf](https://github.com/junegunn/fzf)** - Fuzzy finder for the command line

## Usage

After installation:

1. Reload your shell configuration:
   ```bash
   source ~/.zshrc
   ```

2. Start a new tmux session:
   ```bash
   tmux
   ```

## Customization

Feel free to fork this repository and modify the configurations to suit your needs.

## License

MIT License - feel free to use and modify as needed.
