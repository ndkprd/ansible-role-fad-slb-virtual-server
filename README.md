# ansible-role-fortiadc-slb-virtual-server

## Description

Ansible role to create/update Fortinet's FortiADC SLB Virtual Server entries using REST API.

## Usage

### Install Role

```
ansible-galaxy install ndkprd.fad_slb_virtual_server
```

### Hosts Example

```
[fortiadc]
fad-01 ansible_host=fad-01.infra.ndkprd.com ansible_connection=local fad_apitoken=mysupersecrettoken fad_vdom=root
```

### Playbook Example

See [test folder](tests/).

### About Tags

Each task is tagged with their task file name, `fad_slb_virtual_server`.

There's also a some kind of pre-task and post-task that run before and after create/update tasks to compare the value of before and after create/update tasks, tagged with the above tag and an additional `debug` tag.

## Limitation

Only developed and tested against FortiADC 7.0.

## License

MIT, use at your own risk.
