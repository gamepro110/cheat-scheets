# #Debian based tab auto-completion

## install packages

- bash-completion

```bash
sudo apt install bash-completion
```

## add text to `~/.bashrc`

```bash
if [ -f /etc/bash_completion ]; then
  . /etc/bash_completion
fi
```

> add to end of file
