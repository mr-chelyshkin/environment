# Install zsh
Install zsh/oh-my-zsh

## default.yml

### Modifications:
- Binary Paths:
  - `/usr/bin/zsh`
  - `/usr/bin/git`
- Configuration Path:
  - `{{ zsh_user }}/home/.oh-my-zsh`

> Use default `.zshrc` profile with adding `/etc/profile` content.

### Variables:
- "zsh_user" as default: `{{ ansible_user }}`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions