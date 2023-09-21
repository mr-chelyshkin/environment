# Nvim.
For installing nvim use `snapd`.  
  
For manage nvim version (channel):
```yaml
nvim_version: "latest/stable"
```
Available channels:
```shell
$ snap info nvim
...
channels:
  latest/stable:    v0.9.1                 2023-06-16 (2813) 23MB classic
  latest/candidate: ↑
  latest/beta:      ↑
  latest/edge:      v0.10.0-530+g8376e8700 2023-06-16 (2815) 23MB classic
```
Specify profile [`.bashrc`, `.zshrc`, ...] for add snap and aliases:
```yaml
nvim_profile_path: "/etc/profile"
```
Add alias `vi -> nvim`:
```yaml
nvim_vi_alias: true
```
Add alias `vim -> nvim`:
```yaml
nvim_vim_alias: true
```
Add custom Nvim config:
```yaml
nvim_plugins_repo: "https://github.com/mr-chelyshkin/.nvim"
nvim_plugins_users: [
  "{{ ansible_user }}",
]
```
If `nvim_plugins_repo` is empty: install Nvim config will skip.  
Nvim config install NvChad and clone sources from remote repository to: `/home/[ user in nvim_plugins_users ]/.config/nvim/lua/custom`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
