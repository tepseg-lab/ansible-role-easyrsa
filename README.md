[![CI](https://github.com/tepseg-ab-original/ansible-role-easyrsa/actions/workflows/main.yml/badge.svg)](https://github.com/tepseg-ab-original/ansible-role-easyrsa/actions/workflows/main.yml)
[![Galaxy](https://img.shields.io/badge/galaxy-tepseg-ab.easyrsa-blue.svg)](https://galaxy.ansible.com/tepseg-ab/easyrsa/)

Ansible Role: EasyRSA
=========

Installs EasyRSA 3 and generates certificates and keys.

Requirements
------------

- Ansible >= 2.8 (might work with other versions too)

- This role does **not** need to be run as root, although it supports it.

Role Variables
--------------

See [meta/argument_specs.yml](meta/argument_specs.yml) for a full list of variables together
with documentation on how to use them to configure this role.

For more info on the different key formats that easyrsa can generate, take
a look at [key-formats.md](key-formats.md).

When the role runs, `easyrsa_role_run` (a variable set internally by the role)
is set to true. If `easyrsa_enabled` is set to `false`, the role does not run
and `easyrsa_role_run` will be set to `false`.

Example Playbook
----------------

See [molecule/default/converge.yml](molecule/default/converge.yml) and
[molecule/default/side_effect.yml](molecule/default/side_effect.yml) for
working examples of how to use this role

License
-------

GPLv3

Author Information
------------------

Nikolaos Kakouros
