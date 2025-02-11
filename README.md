# ansible-role-bloodhound #

[![GitHub Build Status](https://github.com/cisagov/ansible-role-bloodhound/workflows/build/badge.svg)](https://github.com/cisagov/ansible-role-bloodhound/actions)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/cisagov/ansible-role-bloodhound.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/cisagov/ansible-role-bloodhound/alerts/)
[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/cisagov/ansible-role-bloodhound.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/cisagov/ansible-role-bloodhound/context:python)

This is an ansible role for installing
[BloodHound](https://github.com/BloodHoundAD/BloodHound).

## Requirements ##

None.

## Role Variables ##

| Variable | Description | Default | Required |
|----------|-------------|---------|----------|
| password | The password used for `neo4j`. | Random password created with the [Ansible password module](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/password_lookup.html). | No |

## Dependencies ##

None.

## Example Playbook ##

Here's how to use it in a playbook:

```yaml
- hosts: all
  become: yes
  become_method: sudo
  roles:
    - bloodhound
```

## Contributing ##

We welcome contributions!  Please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for
details.

## License ##

This project is in the worldwide [public domain](LICENSE).

This project is in the public domain within the United States, and
copyright and related rights in the work worldwide are waived through
the [CC0 1.0 Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0
dedication. By submitting a pull request, you are agreeing to comply
with this waiver of copyright interest.

## Author Information ##

Kyle Evers - kyle.evers@trio.dhs.gov
