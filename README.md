# Ansible Playbooks

# Index
- **Languages**:
    - **[golang](https://github.com/mr-chelyshkin/environment/blob/main/roles/golang/README.md)** [default: `source`]
        - [source](https://github.com/mr-chelyshkin/environment/blob/main/roles/golang/tasks/source.yml): Install goLang from official sources
    - **[nodejs](https://github.com/mr-chelyshkin/environment/blob/main/roles/nodejs/README.md)** [default: `source`]
        - [source](https://github.com/mr-chelyshkin/environment/blob/main/roles/nodejs/tasks/source.yml): install NodeJS from official sources
    - **[python](https://github.com/mr-chelyshkin/environment/blob/main/roles/python/README.md)** [default: `build`]
        - `build`: Build and install python on local machine.
- **CLI Tools**:
    - **[k9s]**
        - [default]
    - **[fzf]**
        - [default]
    - **[network](https://github.com/mr-chelyshkin/rpi4_network_controller/blob/main/README.md)**
      - Tool for manage WiFi connection from terminal.
      - Support Debian, aarch64
- **Utilities**:
    - **[docker](https://github.com/mr-chelyshkin/environment/blob/main/roles/docker/README.md)**
      - Install Docker + Docker-Compose.
    - **[neovim](https://github.com/mr-chelyshkin/environment/blob/main/roles/nvim/README.md)**
      - Install Nvim + NvChad with custom nvim plugins.
    - **[zsh](https://github.com/mr-chelyshkin/environment/blob/main/roles/zsh/README.md)** 
      - Install Zsh + oh-my-zsh plugin.
- **Other**:
  - **[upgrade](https://github.com/mr-chelyshkin/environment/tree/main/roles/upgrade)**
    - Support Debian/RedHat, any arch

