# GoLang.
For manage version to install:
```yaml
golang_version: "1.21.0"
```
For manage installing path:
```yaml
golang_source_path: "/usr/local/go"
```
Specify profile [`.bashrc`, `.zshrc`, `etc`, ...] for add GoEnvs:
```yaml
golang_profile_path: "/etc/profile"
```
More settings in `./vars/{{ file.yml }}`

### Notes
About environment.
```yaml
pattern: {{ golang_source_path }}/go{{ golang_version }}

golang_source_path: "/usr/local/go"
golang_version: "1.21.0"

RESULT: "/usr/local/go/go1.21.0"
GOROOT: "/usr/local/go/go1.21.0"
GOBIN:  "/usr/local/go/bin"
GOPATH: "/usr/local/go/"
```
It's done this way so that you can have multiple different versions of GoLang by changing only GOROOT.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
- Darwin (macOS)
