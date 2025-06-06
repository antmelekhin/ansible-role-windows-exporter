Windows Exporter
================

An Ansible role to install, configure and update the [Windows Exporter](https://github.com/prometheus-community/windows_exporter).

Upgrade to 2.x
--------------

Since the 2.0.0 version of the role, some variables have changed. You will need to update them in your playbooks.

- `windows_exporter_listen_address` to `windows_exporter_web_listen_address`
- `windows_exporter_listen_port` to `windows_exporter_web_listen_port`
- `windows_exporter_metrics_path` to `windows_exporter_telemetry_path`
- `windows_exporter_timeout_margin` to `windows_exporter_scrape_timeout_margin`
- `windows_exporter_max_requests` to `windows_exporter_telemetry_max_requests`

Upgrade to 3.x
--------------

In version 3.0.0, the `windows_exporter_collector` variable was renamed to `windows_exporter_collectors`.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- `pywinrm` is a python library for connection Ansible to Windows hosts via [WinRM](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html).
- `passlib` on a deployer host when using the basic authentication feature (`python3 -m pip install passlib[bcrypt]`).
- `cryptography` or `pyOpenSSL` on a deployer host when using the TLS feature.
- Supported platforms:
  - Windows
    - all

Role Variables
--------------

All variables that can be overridden are stored in the [defaults/main.yml](https://github.com/antmelekhin/ansible-role-windows-exporter/blob/main/defaults/main.yml) file.
Please refer to the [meta/argument_specs.yml](https://github.com/antmelekhin/ansible-role-windows-exporter/blob/main/meta/argument_specs.yml) file for a description of the available variables.
Similarly, descriptions and defaults for preset variables can be found in the [vars/main.yml](https://github.com/antmelekhin/ansible-role-windows-exporter/blob/main/vars/main.yml) file.

Dependencies
------------

When using Ansible core, you will also need to install the following Ansible collections:

```yaml
---
collections:
  - name: community.windows
```

Example Playbook
----------------

Install, configure the `Windows Exporter` and specify a custom query for service collector.

```yaml
---
- name: 'Setup the Windows Exporter'
  hosts: windows_exporter

  roles:
    - role: antmelekhin.windows_exporter
      windows_exporter_collectors_enabled: '[defaults],memory'
      windows_exporter_collectors:
        - name: service
          flags:
            services-where: Name='windows_exporter'
```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
