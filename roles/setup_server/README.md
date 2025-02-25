# infra.osbuild.setup_server

This role automates the setup of a server capable of performing [osbuild](https://www.osbuild.org/)
[compose builds](https://www.osbuild.org/guides/user-guide/user-guide.html)
using the osbuild backend [Weldr](https://weldr.io/) API.

## Requirements

None

## Role Variables

## Variables Exported by the Role

None.

## Dependencies

None.

## Example Playbook

```yaml
---
- name: Run osbuild_builder role to setup obuild compose build server
  become: true
  hosts: all
  tasks:
    - name: Run the role
      ansible.builtin.import_role:
        name: infra.osbuild.setup_server
```

## License

GPLv3
