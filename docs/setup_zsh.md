# Set up ZSH, Oh-My-Zsh

## Configure ZSH to be default shell
Add the following to `.bash_profile`
```bash
export SHELL=/bin/zsh
[ -z "$ZSH_VERSION" ] && exec /bin/zsh -l
```

## Install Oh-My-Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install Powerline10k
1. Download from GitHub
  ```
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
  ```
3. Set `ZSH_THEME="powerlevel10k/powerlevel10k"` in `.zshrc`
