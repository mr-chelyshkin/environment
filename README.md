# Ansible Playbooks
For work with Ansible and this repository playbooks in container, 
you can use image from [project](https://github.com/mr-chelyshkin/ansible-tools):
```shell
docker pull chelyshkin/ansible:latest
docker run --rm -ti chelyshkin/ansible:latest bash
```

### Predefined group: Raspberry
```shell
ansible-playbook -i hosts PiDev.yml \
--user "{{ raspberry_user }}" \
--extra-vars "ansible_ssh_pass={{ raspberry_user_password }}" \
--extra-vars "ansible_become_pass={{ raspberry_sudo_password }}" \
--extra-vars "ansible_host={{ raspberry_host }}"
```
[list of roles](https://github.com/mr-chelyshkin/environment/blob/main/PiDev.yml).  
For manage [roles](https://github.com/mr-chelyshkin/environment/blob/main/group_vars/PiDev.yml) 
change variables or by run ansible-playbook:
```shell
ansible-playbook -i hosts PiDev.yml \
--user "{{ raspberry_user }}" \
--extra-vars "ansible_ssh_pass={{ raspberry_user_password }}" \
--extra-vars "ansible_become_pass={{ raspberry_sudo_password }}" \
--extra-vars "ansible_host={{ raspberry_host }}" \
\
--extra-vars "{{ role_name }}=false" # << -- disable role
```

# Index
- **Languages**:
    - **[golang](https://github.com/mr-chelyshkin/environment/blob/main/roles/golang/README.md)** [default: `source`]
        - [source](https://github.com/mr-chelyshkin/environment/blob/main/roles/golang/tasks/source.yml): Install goLang from official sources
        - Support Debian/RedHat/Darwin, any arch
    - **[nodejs](https://github.com/mr-chelyshkin/environment/blob/main/roles/nodejs/README.md)** [default: `source`]
        - [source](https://github.com/mr-chelyshkin/environment/blob/main/roles/nodejs/tasks/source.yml): install NodeJS from official sources
        - Support Debian/RedHat/Darwin, any arch
    - **[python](https://github.com/mr-chelyshkin/environment/blob/main/roles/python/README.md)** [default: `build`]
        - `build`: Build and install python on local machine.
        - Support Debian/RedHat/Darwin, any arch
- **CLI Tools**:
    - **[k9s](https://github.com/derailed/k9s/blob/master/README.md)**
        - Command-line fuzzy finder
        - Support Debian/RedHat/Darwin, any arch
  - **[fzf](https://github.com/junegunn/fzf/blob/master/README.md)**
      - Kubernetes cli-tool
      - Support Debian/RedHat/Darwin, any arch
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

