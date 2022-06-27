Ansible Role Octopus
=========

Installs Octopus-cli on Debian/Ubuntu servers. 

Role Variables
--------------

```
# Octopus Version to install
octopus_cli_version: ""

# Toggling this will uninstall from the server
uninstall: false
```

Example Playbooks
----------------

Minimal:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.octopuscli
```

Specific Version:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.octopuscli
      vars:
        octopus_cli_version: "9.0.0"
```

Uninstall:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.octopuscli
      vars:
        uninstall: true
```