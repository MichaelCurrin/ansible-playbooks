# Ansible Playbooks
> Manage packages and configurations on my machines using Ansible

Focused on Linux and macOS laptops.


## Resources

## Ansible

- https://ansible.com
- https://docs.ansible.com
    - [Getting Started](https://docs.ansible.com/ansible/latest/user_guide/intro_getting_started.html)

### Installation

- https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html	
- https://linuxhandbook.com/install-ansible-linux/

### Usage tutorials

- https://opensource.com/article/18/3/manage-workstation-ansible
    - https://gitlab.com/jsherman82/ansible_article
- https://opensource.com/article/18/3/manage-your-workstation-configuration-ansible-part-2

### Template repos

- https://github.com/pbulteel/ansible-laptop
- https://github.com/acch/ansible-boilerplate
- https://github.com/dmahler/ansible-template


## Requirements

- [Ansible](https://ansible.com)
- [Git](https://git-scm.com/)


## Installation

### Install system dependencies

- Debian/Ubuntu
    ```sh
    $ sudo apt install -y ansible git
    ```


## Usage

### Ad hoc commands

```sh
$ ansible localhost -m ping
localhost | SUCCESS => {
    "changed": false,
    "ping": "pong"
}
```

```sh
$ ansible localhost -a "/bin/echo hello"
localhost | CHANGED | rc=0 >>
hello
```


### Run the playbook

```sh
$ sudo ansible-pull -U https://github.com/MichaelCurrin/ansible-playbooks.git local.yml
```
