# podman-pihole

## Set up
Copy the service unit file to `/etc/systemd/system`.

### Run the following.

_Configure SELinux to allow systemd to load containers._

```bash
setsebool -P container_manage_cgroup on
```

_Tell systemd to start the pihole container automatically_

```bash
systemctl --now enable pihole.service
```
