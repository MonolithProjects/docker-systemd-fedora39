# Fedora 39 Ansible Test Image

[![Dockerfile test](https://github.com/MonolithProjects/docker-systemd-fedora39/actions/workflows/main.yml/badge.svg)](https://github.com/MonolithProjects/docker-systemd-fedora39/actions/workflows/main.yml)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora39)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora39)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora39)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora39)
[![DockerHub](https://img.shields.io/docker/image-size/monolithprojects/systemd-fedora39?sort=date)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora39)

Docker image with Fedora 39 and enabled systemd. Image is updated with the latest software updates on the 1st day in the month. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  

**Note:** This docker image is ment to be used for Molecule Ansible tests and development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora39/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-fedora39:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-fedora39:latest`  

## License

MIT
