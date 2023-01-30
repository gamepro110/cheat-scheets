# use sshkeys from windows in wsl

>all in wsl terminal

## copy over

```bash
cp /mnt/c/User/<UserName>/.ssh/<path_to_key>* ~/.ssh/
```

## set correct ownership and permissions

```bash
sudo chown <username> ~/.ssh/<keyname>* && \
sudo chmod 600 ~/.ssh/<keyname>*
```

## add them to the ssh-agent

```bash
eval "$(ssh-agent -s)" && ssh-add ~/.ssh/<key>
```
