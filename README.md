# Stacc ASCII Art for Neofetch

Be welcomed by a fresh looking shell every time you open your terminal.

![Preview](/preview.png)

## Setup

### 1. Install Neofetch

First, install [Neofetch](https://github.com/dylanaraps/neofetch). Click [here](https://github.com/dylanaraps/neofetch/wiki/Installation) for detailed instructions.

On macOS.

```bash
brew install neofetch
```

On Ubuntu.

```bash
sudo apt update && sudo apt install neofetch
```

### 2. Clone this repo and open folder

```bash
git clone git@github.com:stacc-as/stacc-neofetch.git
cd stacc-neofetch
```

### 3. Copy ascii art

```bash
mkdir -p ~/.config/neofetch/ascii-art && cp logos/* $_
```

### 4. Pick a logo

There are several logos available, pick your favorite.

```bash
export LOGO=stacc.txt
# or
export LOGO=stacc-pride.txt
```

### 5. Add Neofetch to shell config

For bash.

```bash
echo "neofetch --ascii ~/.config/neofetch/ascii-art/$LOGO" >> ~/.bashrc
```

For zsh.

```zsh
echo "neofetch --ascii ~/.config/neofetch/ascii-art/$LOGO" >> ~/.zshrc
```

### 6. All done

Reload your shell and continue working! ☕️
