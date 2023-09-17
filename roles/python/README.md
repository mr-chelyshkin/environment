# Install python
Install python

## linux.source.yml
Downloads and build from official source, <b>it's take a time</b>.

### Modifications:
- Binary Paths:
  - `/usr/local/bin/python{{ python_version }}`
  - `/usr/local/bin/pip3`
  - `/usr/bin/ccache`
  - `/usr/bin/make`
  - `/usr/bin/gcc`
- Common:
  - `zlib-devel` development files for the zlib compression library
  - `libffi-devel` development files for the Foreign Function Interface library
  - `openssl-devel` development files for OpenSSL

### Variables:
- "python_version" as default: `3.11.4`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions