Docker
======

An Ansible role to install [Docker Engine](https://docs.docker.com/engine/) from the Docker repository and configure it.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- Supported platforms:
  - Debian
    - 10
    - 11
    - 12
  - Fedora
    - 39
    - 40
  - RHEL
    - 7
    - 8
    - 9
  - Ubuntu
    - 18.04
    - 20.04
    - 22.04

Role Variables
--------------

All variables that can be overridden are stored in the [defaults/main.yml](https://github.com/antmelekhin/ansible-role-docker/blob/main/defaults/main.yml) file.
Please refer to the [meta/argument_specs.yml](mhttps://github.com/antmelekhin/ansible-role-docker/blob/main/meta/argument_specs.yml) file for a description of the available variables.
Similarly, descriptions and defaults for preset variables can be found in the [vars/main.yml](https://github.com/antmelekhin/ansible-role-docker/blob/main/vars/main.yml) file.

Dependencies
------------

None.

Example Playbook
----------------

Install Docker Engine:

```yaml
---
- name: 'Install Docker Engine'
  hosts: all

  roles:
    - role: antmelekhin.docker
```

Install Docker Engine and configure a DNS server for all Docker containers:

```yaml
---
- name: 'Install Docker Engine'
  hosts: all

  roles:
    - role: antmelekhin.docker
      docker_daemon_options:
        dns:
          - '8.8.8.8'
        dns-search:
          - 'example.com'
```

Install Docker Engine v23.0.6:

```yaml
---
- name: 'Install Docker Engine v23.0.6'
  hosts: all

  roles:
    - role: antmelekhin.docker
      docker_version: '5:23.0.6-1~ubuntu.22.04~jammy'
      when: ansible_distribution == 'Ubuntu' and ansible_distribution_version is version('22.04', '=')

    - role: antmelekhin.docker
      docker_version: '23.0.6'
      when: ansible_os_family == 'RedHat'
```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
