# Zsh.
Install zsh and oh-my-zsh plugin.

Specify the users for using zsh:
```yaml
zsh_users: [
  "{{ ansible_user }}",
]
```
Manage `oh-my-zsh` installation:
```yaml
zsh_oh_my_zsh_plugin: true
```

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
