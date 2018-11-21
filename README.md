# Ansible Role: Containerized TACACS+ Server

Installs TACACS+ (lfkeitel/tacacs_plus) inside a Docker container. Only usable with Docker Compose version 3.

## Role Variables

See `defaults/main.yml`.


## Add to Requirements

    - src: https://github.com/nexcess/ansible-role-tacacs.git
      name: nexcess.tacacs
    - src: https://github.com/geerlingguy/ansible-role-docker.git
      name: geerlingguy.docker

## Example Playbook

    - hosts: tacacs_hosts
      roles:
        - nexcess.tacacs
        - geerlingguy.docker

## License

MIT
