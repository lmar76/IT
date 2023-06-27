# Docker

## Daemon configuration

Reference: https://docs.docker.com/config/daemon/

Configuration file:
- on Linux: `/etc/docker/daemon.json`

## Daemon data directory

Daemon data directory is stored by defaul:
- on Linux: in `/var/lib/docker`
- on Windows: in `C:\ProgramData\docker`

Different paths can be specified using the `data-root` configuration parameter. E.g.:

```json
{
  "data-root": "/mnt/docker-data"
}
```

Reference: https://docs.docker.com/config/daemon/#daemon-data-directory

## Run a container in interactive mode

```sh
docker run -i -t [docker_image]
```

## Override entrypoint with docker run

```sh
docker run --entrypoint [new_command] [docker_image]
```
