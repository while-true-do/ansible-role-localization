[![Build Status](https://travis-ci.org/while-true-do/ansible-role-localization.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-localization)

# Ansible Role: localization
| A role to set the localization and keymap.

## Motivation

Having a proper configuration of keymap and localization is a very common task.

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/while-true-do/localization)

```
ansible-galaxy install while-true-do.localization
```

Install from [Github](https://github.com/while-true-do/ansible-role-localization)

```
git clone https://github.com/while-true-do/ansible-role-localization.git while-true-do.localization
```

## Requirements

Used Modules:

-  [command_module](http://docs.ansible.com/ansible/latest/command_module.html)
-  [shell_module](http://docs.ansible.com/ansible/latest/shell_module.html)
-  [template_module](http://docs.ansible.com/ansible/latest/template_module.html)

## Dependencies

None.

## Role Variables

```yaml
wtd_locale_lang: "en_US.utf8"
wtd_locale_keymap: "us"

# Unset variables, but you can use them in your tasks, vars or so
wtd_locale_lc_address: ""
wtd_locale_lc_collate: ""
wtd_locale_lc_ctype: ""
wtd_locale_lc_identification: ""
wtd_locale_lc_measurement: ""
wtd_locale_lc_messages: ""
wtd_locale_lc_monetary: ""
wtd_locale_lc_name: ""
wtd_locale_lc_numeric: ""
wtd_locale_lc_paper: ""
wtd_locale_lc_telephone: ""
wtd_locale_lc_time: ""
```

## Example Playbook

Simple Example:

```
- hosts: servers
  roles:
  - { role: while-true-do.localization }
```

## Testing

All tests should be put in [test directory](./tests/).

## Contribute / Bugs

Thank you so much for considering to contribute. Every contribution helps us.
We are really happy, when somebody is joining the hard work. Please have a look
at the links first.

-   [Contribution Guidelines](./docs/CONTRIBUTING.md)
-   [Create an issue or Request](https://github.com/while-true-do/ansible-role-localization/issues)
-   [See who was contributing already](https://github.com/while-true-do/ansible-role-localization/graphs/contributors)

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Author Information

Blog: [blog.while-true-do.org](https://blog.while-true-do.org)

Mail: [hello@while-true-do.org](mailto:hello@while-true-do.org)

