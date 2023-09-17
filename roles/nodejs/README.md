# Install nodejs
Install nodejs

## linux.source.yml
Downloads Node.js from its official source and extracts it to a system-wide location.

### Modifications:
- Binary Paths:
  - `/usr/local/node/bin/node`
  - `/usr/local/node/bin/npm`
  - `/usr/local/node/bin/npx`
- Configuration Changes:
  - `libffi-devel` development files for the Foreign Function Interface library
  - `/usr/local/node/bin` added to the system PATH in `/etc/profile`
  - `openssl-devel` development files for OpenSSL

### Variables:
- "nodejs_version" as default: `20.5.1`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions