# Prepare raspberry
Update packages and add dependencies.

## raspbian.devel.yml

### Modifications:
- Binary Paths:
  - `/usr/bin/snap`
  - `/usr/bin/make`
  - `/usr/bin/gcc`
  - `/usr/bin/git`
  - `/usr/bin/jq`
- Library:
  - `libiw-dev` C-library for wireless network operations.
- Common tools:
  - `/usr/bin/network` - console [tool](https://github.com/mr-chelyshkin/rpi4_network_controller) for manage wireless connection

### Supported Platforms:
 - Debian-based Linux distributions (arm64 architecture)
 - RedHat-based Linux distributions (arm64 architecture)
