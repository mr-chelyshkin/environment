# Install nvim
Install nvim and nvChad with plugins as optional.

## default.yml
Install nvim.

### Modifications:
- Binary Paths:
  - `/usr/bin/snap`
  - `/snap/bin/nvim`
- Configuration Path:
  - uses `/etc/profile` to add aliases for both vi / vim to point to `/snap/bin/nvim`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions

## with_plugins.yml
Install nvim, nvChad and plugins from sources.

### Modifications:
- Binary Paths:
  - `/usr/bin/snap`
  - `/snap/bin/nvim`
- Configuration Path:
  - uses `/etc/profile` to add aliases for both vi / vim to point to `/snap/bin/nvim`.
  - add plugins to `{{ ansible_env.HOME }}/.config/nvim/lua/custom` from `nvim_plugins_repo`
  - `{{ ansible_env.HOME }}/.config/nvim`

### Variables:
- "nvim_plugins_repo" as default: `https://github.com/mr-chelyshkin/.nvim`.

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions