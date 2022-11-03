in file `/etc/dhcpcd.conf` add the following at the bottom

```conf
interface {{interface}}
static ip_address={{static-ip}}/{{netmask}}
static routers={{router-ip}}
static domain_name_servers={{dns-ip}}
```

| {{tag}}       | descrition                                                         |
| ------------- | ------------------------------------------------------------------ |
| {{interface}} | network interface used to set static ip (eth0 = default rpi wired) |
| {{netmask}}   | netmask to apply (`/24` for `255.255.255.0`)                                                                   |
| {{static-ip}} | the static ip for this interface                                   |
| {{router-ip}} | gateway, ip of your router                                         |
| {{dns-ip}}    | dns address for domain name resolution                             |

reboot to make it take effect

## example

```conf
interface eth0
static ip_address=192.168.0.5/24
static routers=192.168.0.1
static domain_name_servers=1.1.1.1
```
