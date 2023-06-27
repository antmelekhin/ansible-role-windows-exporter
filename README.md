Windows Exporter
================

An Ansible role for install, configure and update [Windows Exporter](https://github.com/prometheus-community/windows_exporter).

Requirements
------------

- Supported version of Ansible: 2.9 and highter.
- `pywinrm` is a python library for connection Ansible to Windows hosts via [WinRM](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html).
- Supported platforms:
  - Windows
    - 2016
    - 2019

Role Variables
--------------

- `windows_exporter_version` The specific version of Windows Exporter to download (default: `0.22.0`).
- `windows_exporter_package_name` Windows Exporter package name (default: `windows_exporter-0.22.0-amd64.msi`).
- `windows_exporter_download_url` URL to download Windows Exporter package (default: `https://github.com/prometheus-community/windows_exporter/releases/download/v0.22.0`).
- `windows_exporter_listen_address` The IP address to bind to (default: `0.0.0.0`).
- `windows_exporter_listen_port` The port to bind to (default: `9182`).
- `windows_exporter_metrics_path` The path at which to serve metrics (default: `metrics`).
- `windows_exporter_log_level` Windows Exporter logging level (default: `info`).
- `windows_exporter_collectors_enabled` Comma-separated list of collectors to use (default: `[defaults]`).
- `windows_exporter_collector` Flags for collectors (default: `''`).
- `windows_exporter_tls_server_config` Certificate and key files for server to use to authenticate to client.
- `windows_exporter_http_server_config` Enable HTTP/2 support. Note that HTTP/2 is only supported with TLS.
- `windows_exporter_basic_auth_users` Users and password for basic authentication. Passwords are automatically hashed with bcrypt.

Dependencies
------------

None.

Example Playbook
----------------

Install, configure `Windows Exporter` and specify a custom query for service collector.

  ```yaml
  ---
  - name: 'Setup Windows Exporter'
    hosts: windows_exporter

    roles:
      - role: antmelekhin.windows_exporter
        windows_exporter_collectors_enabled: '[defaults],memory'
        windows_exporter_collector:
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
