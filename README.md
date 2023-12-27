Docker
======

An Ansible role for install Docker Engine.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- Supported platforms:
  - Debian
    - 10
    - 11
    - 12
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

- `docker_repository_mirror` Mirror of `Docker` repository (default: `https://download.docker.com/linux`).
- `docker_repository_release_channel` `Docker`release channel.

  Available values:
  - `stable` (default)
  - `test`

- `docker_version` The specific version of Docker Engine to install. By default, role install latest version.
- `docker_users` A list of users who will be added to the docker group (default: `[]`).

Dependencies
------------

None.

Example Playbook
----------------

- Install `Docker Engine`:

  ```yaml
  ---
  - name: 'Install Docker Engine'
    hosts: all

    roles:
      - role: antmelekhin.docker
  ```

- Install `Docker Engine` v23.0.6:

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
        when: ansible_os_family == 'RedHat' and ansible_distribution_major_version is version('8', '>=')
  ```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
