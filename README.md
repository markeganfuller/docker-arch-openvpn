# Docker Archlinux OpenVPN

[![Dockerhub Build](https://img.shields.io/docker/cloud/build/mefdock/docker-arch-openvpn)](https://cloud.docker.com/repository/docker/mefdock/docker-arch-openvpn)

Docker container using Archlinux and providing [OpenVPN](https://openvpn.net/)

This container is meant to connect to a VPN without affecting the hosts
networking and provide the VPN connection to other containers e.g. via
docker-compose `network_mode: service:openvpn`

## Usage

Configuring a VPN requires `NET_ADMIN` capabilities therefore the container
must be run with:

```
--cap_add NET_ADMIN
```
