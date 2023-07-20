# changing #debian 12 to static ip

## in `/etc/network/interfaces`

```conf
# This file describes the network interfaces available on your system
# and how to activate them. For more information, see interfaces(5).

source /etc/network/interfaces.d/*

# The loopback network interface
auto lo
iface lo inet loopback

# The primary network interface
allow-hotplug ens18
iface ens18 inet dhcp
```

change it to

```conf
# This file describes the network interfaces available on your system
# and how to activate them. For more information, see interfaces(5).

source /etc/network/interfaces.d/*

# The loopback network interface
auto lo
iface lo inet loopback

# The primary network interface
auto ens18
iface ens18 inet static
  address 192.168.30.61 # change to required ip
  netmask 255.255.255.0 # change to required netmask
  gateway 192.168.30.254 # change to required gateway
  dns-nameservers 192.168.30.10 # change to required dns-server
```
