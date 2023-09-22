# NodeJS.
For manage version to install:
```yaml
nodejs_version: "20.5.1"
```
For manage installing path:
```yaml
nodejs_source_path: "/usr/local/node"
```
Specify users and profiles [`.bashrc`, `.zshrc`, `etc`, ...] for add Node Envs:
```yaml
nodejs_users: [
  "{{ ansible_user }}"
]
profiles: [
  "/etc/profile"
]
```
More settings in `./vars/{{ file.yml }}`

### Notes
About environment.
```yaml
pattern: {{ nodejs_source_path }}/node{{ nodejs_version }}

nodejs_source_path: "/usr/local/node"
nodejs_version: "20.5.1"

RESULT: "/usr/local/node/node20.5.1"
```
It's done this way so that you can have multiple different versions of NodeJS.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
- Darwin (macOS)
