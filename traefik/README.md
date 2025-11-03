# Lograte 
place this example code at `/etc/logrotate.d/traefik` on your docker host server
please adjust the custom file path below, where your traefik logs are stored
please adjust the below traefik container name to send the USR1 signal for log rotation
https://blog.lrvt.de/configuring-crowdsec-with-traefik/#enabling-traefik-logs

`$ lograte -f traefik`


```bash
compress
/mnt/truenas/docker_data/traefik/logs/*.log {
  size 20M
  daily
  rotate 14
  missingok
  notifempty 
  postrotate
  docker kill --signal="USR1" traefik # adjust this line to your traefik container name
  endscript
}
```
