# Containers

## Docker

### Address Pools

See: https://straz.to/2021-09-08-docker-address-pools/

### Daemon configuration

Reference: https://docs.docker.com/config/daemon/

Configuration file:

- on Linux: `/etc/docker/daemon.json`

### Daemon data directory

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

### Run a container in interactive mode

```sh
docker run -i -t [docker_image]
```

### Override entrypoint with docker run

```sh
docker run --entrypoint [new_command] [docker_image]
```

## Open Container Initiative

The Open Container Initiative is an open governance structure for the express purpose of
creating open industry standards around container formats and runtimes.

Web site: https://opencontainers.org/

- OCI Image Manifest Specification: https://github.com/opencontainers/image-spec/blob/main/manifest.md
- GitHub project: https://github.com/opencontainers
