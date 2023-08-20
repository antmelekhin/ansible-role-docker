Docker
======

An Ansible role for install Docker Engine.

Requirements
------------

- Supported version of Ansible: 2.9 and highter.
- Supported platforms:
  - Debian
    - 10
    - 11
    - 12
  - RHEL
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

License
-------

MIT

Author Information
------------------

Melekhin Anton.
