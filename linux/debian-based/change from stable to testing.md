---
tags: linux, debian, updates
---

# Debian change from stable to testing

in `/etc/apt/sources.list`

## default example (on pi)

```conf
deb http://deb.debian.org/debian bullseye main contrib non-free
deb http://security.debian.org/debian-security bullseye-security main contrib non-free
deb http://deb.debian.org/debian bullseye-updates main contrib non-free
```

change `bullseye` to `testing`

```conf
deb http://deb.debian.org/debian testing main contrib non-free
deb http://security.debian.org/debian-security testing-security main contrib non-free
deb http://deb.debian.org/debian testing/updates main contrib non-free
```

## after

run

```bash
sudo apt update && sudo apt upgrade -y
```
