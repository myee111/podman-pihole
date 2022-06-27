# podman-pihole

## Set up
Copy the service unit file to `/etc/systemd/system`.

### Run the following.

__Configure SELinux to allow systemd to load containers.__

```bash
setsebool -P container_manage_cgroup on
```

__Tell systemd to start the pihole container automatically__

```bash
systemctl --now enable pihole.service
```
