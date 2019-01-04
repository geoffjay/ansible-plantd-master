# Ansible Role: Plantd Master

Installs and configures a Plantd master server on a Debian host.

## Requirements

A working installation of `go`.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
plantd_master_version: "0.1.0"
```

## Dependencies

None

## Example Playbook

```yml
- hosts: master
  become: yes
  vars_files:
    - vars/main.yml
  roles:
    - geoffjay.plantdmaster
```

Inside `vars/main.yml`:

```yml
plantd_master_version: "0.1.0"
```

## License

MIT/BSD

## Author Information

This role was created in 2019 by Geoff Johnson.
