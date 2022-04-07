# PHP automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-php
  name: ansible-role-php
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-php

- Import role and override role variables, e.g.
```
- name: Setup php
  roles:
    - role: ansible-role-php
```

- All available role vars can be found in `defaults`
