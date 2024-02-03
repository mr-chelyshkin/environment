# Docker.
For manage packages / editions:
```yaml
docker_edition: 'ce'
docker_packages:
  - "docker-{{ docker_edition }}"
  - "docker-{{ docker_edition }}-cli"
  - "docker-{{ docker_edition }}-rootless-extras"
```
For manage Docker-Compose installing:
```yaml
docker_install_compose: true / false
docker_compose_version: "v2.21.0"
```
Specify the users who should be added to the `docker` group:
```yaml
docker_users: [
  "{{ ansible_user }}"
]
```
Manage Docker daemon options `/etc/docker/daemon.json`
```yaml
docker_daemon_options:
  storage-driver: "overlay2"
  log-opts:
    max-size: "20m"
```
More settings in `./vars/{{ file.yml }}`

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
