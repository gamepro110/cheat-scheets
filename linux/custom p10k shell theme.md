## packages

### debian
	- zsh
	- zsh-common
---
### arch-based
	- zsh
	- zsh-autosuggestions
	- zsh-syntax-highlighting
	- zsh-completions
	- zsh-history-substring-search
	- zsh-theme-powerlevel10k
---

## steps

- Install packages
	- found above
- clone p10k repo
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
```
- add p10k theme to `.zshrc`
```bash
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >> ~/.zshrc
```
- start zsh and finish setup
```bash
zsh
```
- copy `.p10k.zsh` from git repo/other pc to destination machine
```bash
scp .p10k.zsh pi-runner:~/.p10k.zsh
```
- set zsh as default shell
```bash
export temp_new_shell=$(which zsh) && chsh -s $temp_new_shell
```
