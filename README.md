# Ansible Role: ansible-role-tester (art) tester

This role is a dummy role used to exercise the various aspects of [ansible-role-tester](https://github.com/fubarhouse/ansible-role-tester).

## Scenarios

- `ansible-role-tester full --playbook tests/playbook-simple.yml` - tests basic functionality.
- `ansible-role-tester full --playbook tests/playbook-library.yml --library "$(pwd)/tests/library"` - depends on a dummy module, which is mounted using the `--library` path in art
- `ansible-role-tester full --playbook tests/playbook-extra-roles.yml --extra-roles /etc/ansible/roles` - test mounting of roles location.
- `ansible-role-tester full --playbook tests/playbook-extra-roles.yml --requirements tests/requirements.yml`
