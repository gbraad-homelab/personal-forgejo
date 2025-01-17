Forgejo for private/internal use in (Bootable) Containers
=========================================================


```bash
$ podman run -d --name forgejo --hostname ${HOSTNAME}-forgejo \
    --net=ncentre-bridge --ip 10.0.21.150 \
    --cap-add=NET_ADMIN --cap-add=NET_RAW --device=/dev/net/tun --cap-add AUDIT_CONTROL \
    ghcr.io/gbraad-homelab/forgejo:latest
```
