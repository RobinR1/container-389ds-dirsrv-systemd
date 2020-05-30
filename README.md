# Systemd service file to run 389ds/dirsrv container via systemd and podman

* `/etc/sysconfig/container-389ds-dirsrv` contains generic settings
* `/etc/389ds-dirsrv-secrets/DS_DM_PASSWORD` is a file for setting the Directory Manager password of the 389 Directory server.
  It should not be readable by anyone but root user and it is highly recommended to remove this file after initialization of the container. This location can be altered via `SECRETS_DIR`
  in the `/etc/sysconfig/container-389ds-dirsrv` file.