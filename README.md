# Amtega login_defs role

Configure local password policy through login.defs file.

## Requirements

- Ansible >= 2.4

## Role Variables

~~~ yaml
pass_max_days: 120
pass_min_days: 0
pass_min_len: 8
pass_warn_age: 7
pass_always_warn: yes
pass_change_tries: 5
~~~

## Dependencies

None.

## Example Playbook

```yaml
---

  - hosts: localhost
    become: true
    roles:
    - role: amtega.login_defs
```

## Testing

Test are based on docker containers. You can run the tests with the following commands:

```shell
$ cd amtega.login_defs/test
$ ansible-playbook main.yml -K
```

## License

Copyright (C) <YEAR> AMTEGA - Xunta de Galicia

This role is free software: you can redistribute it and/or modify
it under the terms of:
GNU General Public License version 3, or (at your option) any later version;
or the European Union Public License, either Version 1.2 or – as soon
they will be approved by the European Commission ­subsequent versions of
the EUPL;

This role is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details or European Union Public License for more details.

## Author Information

- author_name 1 ([mail_adrress_1](mailto:mail_address_1))
- author_name N ([mail_adrress_N](mailto:mail_address_N))
