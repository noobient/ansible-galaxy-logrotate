# bviktor.logrotate

## Synopsys

This role lets you enable log rotation for log files.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `path` | yes | `/var/log/foo.log` | Log file to rotate. |

## Examples

```yml
- include_role:
    name: bviktor.logrotate
  vars:
    path: '/var/log/foo.log'
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-9.yml) |
| Fedora 37 | ✅ | [![Fedora 37](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-37.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-37.yml) |
| Ubuntu 18.04 | ✅ | [![Ubuntu 18.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-18.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-18.04.yml) |
| Ubuntu 20.04 | ✅ | [![Ubuntu 20.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-20.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-20.04.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-22.04.yml) |
