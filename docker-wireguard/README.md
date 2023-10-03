This is based on this [docker-wireguard](https://github.com/linuxserver/docker-wireguard).

## Systems without `iptables-legacy`

In modern versions of Fedora [docker-wireguard](https://github.com/linuxserver/docker-wireguard) doesn't work out of the box. You need to run the following command before starting the container:

```
sudo modprobe iptable_filter
docker compose up
``` 

For more information refer to this [link](https://github.com/linuxserver/docker-wireguard/issues/138#issuecomment-1003173623).
