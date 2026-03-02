# noobient.logrotate

## Synopsys

This role enables log rotation for log files. Rotation occurs daily, and the files are compressed using the XZ compression.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `name` | yes | `tomcat` | Nickname of the log rotation configuration. |
| `pattern` | yes | `/var/log/foo.log` | Pattern(s) for the file(s) to rotate. You can specify multiple patterns, one line per pattern, see examples for syntax. |
| `retention` | no | `14` | Number of days to keep the rotated log files. Defaults to 7. |

## Examples

```yml
- include_role:
    name: noobient.logrotate
  vars:
    name: kf2-ddos
    pattern: /var/log/kf2-ddos.log

- include_role:
    name: noobient.logrotate
  vars:
    name: tomcat
    pattern: |-
      /opt/tomcat/logs/*.log
      /opt/tomcat/logs/catalina.out
    retention: 14
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-9.yml) |
| AlmaLinux 10 | ✅ | [![AlmaLinux 10](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-10.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/almalinux-10.yml) |
| Fedora 42 | ✅ | [![Fedora 42](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-42.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-42.yml) |
| Fedora 43 | ✅ | [![Fedora 43](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-43.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/fedora-43.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-22.04.yml) |
| Ubuntu 24.04 | ✅ | [![Ubuntu 24.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-24.04.yml) |
| Ubuntu 26.04 | ✅ | [![Ubuntu 26.04](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-26.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-logrotate/actions/workflows/ubuntu-26.04.yml) |
