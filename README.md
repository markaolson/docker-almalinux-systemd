# docker-almalinux-systemd

Dockerfile that creates an AlmaLinux image with systemd installed.

The Docker image is intended to be used with Molecule for testing ansible roles.


## Branches

Each branch in this repository contains a Dockerfile for a specific image version.

| Branch | Version | Docker image tag |
| ------ | ------- | ---------------- |
| 8.5    | 8.5     | 8.5              |
| main   | latest  | latest           |


## Run a container

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  markaolson/alma-systemd:latest
```
