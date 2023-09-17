# Install docker
Install docker.

## linux.source.yml
Install Docker from sources.

### Modifications:
- Binary Paths:
  - `/usr/bin/docker`
  - `/usr/bin/dockerd`
- Configuration Changes:
  - Added `docker` group
  - Current ansible user added to the `docker` group

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions