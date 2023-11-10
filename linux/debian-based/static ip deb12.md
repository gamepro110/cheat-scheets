# changing #debian 12 to static ip

>example

```bash
sudo nmcli c show
sudo nmcli c mod 'Wired connection 1' ipv4.addresses 10.10.30.19/24 ipv4.method manual
sudo nmcli con mod 'Wired connection 1' ipv4.gateway 10.10.30.1
sudo nmcli con mod 'Wired connection 1' ipv4.dns "10.10.30.1"
sudo nmcli c down 'Wired connection 1' && sudo nmcli c up 'Wired connection 1'
```

## reverting

```bash
sudo nmcli con modify 'Wired connection 1' ipv4.method auto
```
