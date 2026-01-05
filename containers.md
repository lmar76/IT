# Containers

## Docker

### Address Pools

See: <https://straz.to/2021-09-08-docker-address-pools/>

### Daemon configuration

Reference: <https://docs.docker.com/config/daemon/>

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

Reference: <https://docs.docker.com/config/daemon/#daemon-data-directory>

## Command-line how to

The following commands are referrede to Docker but they are also valid for Podman.

### List of images having empty `Repository` or `Tag`:

```sh
docker images --filter dangling=true
```

### Override entrypoint with docker run

```sh
docker run --entrypoint [new_command] [docker_image]
```

### Run a container in interactive mode

```sh
docker run -i -t [docker_image]
```

### Swap usage

To enable the swap memory usage during the container execution, see <https://docs.docker.com/config/containers/resource_constraints/#--memory-swappiness-details>


## Kubernetes

Official site: <https://kubernetes.io/>.

Alternative distributions:

- minikube: <https://minikube.sigs.k8s.io/docs/>
- K3s: <https://k3s.io/>


## Open Container Initiative

The Open Container Initiative is an open governance structure for the express purpose of
creating open industry standards around container formats and runtimes.

Web site: <https://opencontainers.org/>

- OCI Image Manifest Specification: <https://github.com/opencontainers/image-spec/blob/main/manifest.md>
- GitHub project: <https://github.com/opencontainers>
