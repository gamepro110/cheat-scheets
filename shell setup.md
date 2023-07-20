---
tags: linux, shell, bash, zsh
---

# custom shell setup

## packages

### Debian

- zsh
- zsh-common

### arch

- zsh
- zsh-autosuggestions
- zsh-syntax-highlighting
- zsh-completions
- zsh-history-substring-search
- zsh-theme-powerlevel10k

## steps

- install packages
  - found above
- copy.p10k.zsh file from Code_Snippets/linux/.p10k.zsh to target device
- change shell

  ```bash
  chsh -s <path-to-shell-executable>
  ```

- clone p10k repo

  ```bash
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
  ```

- copy theme from repo

  ```bash
  echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >> ~/.zshrc
  ```

- replace.p10k.zsh with the one from Code_Snippets
