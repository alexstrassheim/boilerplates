# MDNS Setting within TrueNAS
```bash
/etc/avahi/avahi-daemon.conf
disallow-other-stacks=no
service avahi-daemon restart
avahi-browse -a | grep -i matter
```

