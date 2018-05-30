Ansible role docker-login
=========
Ansible role that grants user access to a private docker registry.
It performs a simple docker login command.

Requirements
------------
Docker is required.

Role Variables
--------------
- `docker_registry_url` - sets docker registry endpoint.
- `docker_registry_username` - sets docker registry user name.
- `docker_registry_password` - sets docker registry password.

Dependencies
------------

Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: docker-login,
                docker_registry_url: <registry-endpoint>
                docker_registry_username: <registry-user-name>
                docker_registry_password: <registry-password>
           }

License
-------
MIT/BSD
