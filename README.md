# Ansible Role: localization
| A Role to set the localization and keymap.

## Installation

Galaxy Link: <https://galaxy.ansible.com/while-true-do/localization>

```
ansible-galaxy install while-true-do.localization
```

Github Link: <https://github.com/while-true-do/ansible-role-localization>

```
git clone https://github.com/while-true-do/ansible-role-localization while-true-do.localization
```

## Requirements

None.

## Dependencies

None.

## Role Variables

```
# defaults/main.yml
locale_lang: en_US.utf8
locale_keymap: us

# Unset variables, but you can use them in your tasks, vars or so
# locale_lc_address: ''
# locale_lc_collate: ''
# locale_lc_ctype: ''
# locale_lc_identification: ''
# locale_lc_measurement: ''
# locale_lc_messages: ''
# locale_lc_monetary: ''
# locale_lc_name: ''
# locale_lc_numeric: ''
# locale_lc_paper: ''
# locale_lc_telephone: ''
# locale_lc_time: ''
```

## Example Playbook

Simple Example:

```
- hosts: servers
  roles:
  - { role: while-true-do.localization }
```

Advanced Example:

```
- hosts: servers
  roles:
  - { role: while-true-do.localization, locale_lang: de_DE.utf8, locale_lc_name: de_DE.utf8, locale_keymap: de-nodeadkeys }
```

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Contribute / Bugs

**bug reports:** <https://github.com/while-true-do/ansible-role-localization/issues>

**contributers:** <https://github.com/while-true-do/ansible-role-localization/graphs/contributors>

## Author Information

**blog:** <https://blog.while-true-do.org>

**github:** <https://github.com/daniel-wtd>

**contact:** [mail@while-true-do.org](mailto:mail@while-true-do.org)
