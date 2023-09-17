# Install golang
Install golang

## linux.source.yml
Downloads Go from its official source and sets up the environment for development.

### Modifications:
- Binary Paths:
  - `/usr/local/go/bin/go`
  - `/usr/local/go/bin/gofmt`
- Configuration Changes:
  - `/usr/local/go/bin` added to the system PATH in `/etc/profile`
  - set up GOBIN to `{{ ansible_env.HOME }}/go/bin`
  - set up GOPATH to `{{ ansible_env.HOME }}/go`
  - defined GOROOT as `/usr/local/go`

### Variables:
- "golang_version" as default: `1.21.0`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions