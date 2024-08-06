Windows Exporter
================

An Ansible role to install, configure and update the [Windows Exporter](https://github.com/prometheus-community/windows_exporter).

Update to 2.x
-------------

Since the 2.0.0 version of the role, some variables have changed. You will need to update them in your playbooks.

- `windows_exporter_listen_address` to `windows_exporter_web_listen_address`
- `windows_exporter_listen_port` to `windows_exporter_web_listen_port`
- `windows_exporter_metrics_path` to `windows_exporter_telemetry_path`
- `windows_exporter_timeout_margin` to `windows_exporter_scrape_timeout_margin`
- `windows_exporter_max_requests` to `windows_exporter_telemetry_max_requests`

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

- `windows_exporter_version` The version of Windows Exporter to install (default: `0.26.2`).
- `windows_exporter_package_name` The Windows Exporter package name (default: `windows_exporter-0.26.2-amd64.msi`).
- `windows_exporter_download_url` The Windows Exporter package download URL (default: `https://github.com/prometheus-community/windows_exporter/releases/download/v0.26.2`).
- `windows_exporter_checksum_url` The Windows Exporter checksum file URL (default: `{{ windows_exporter_download_url }}/sha256sums.txt`).
- `windows_exporter_download_path` Local path to download the Windows Exporter package (default: `/tmp`).
- `windows_exporter_web_listen_address` The address to listen for the web interface and telemetry (default: `0.0.0.0`).
- `windows_exporter_web_listen_port` The port number that Windows Exporter listens on (default: `9182`).
- `windows_exporter_scrape_timeout_margin` Seconds to subtract from the timeout allowed by the client (default: `0.5`).
- `windows_exporter_telemetry_path` The path to expose metrics (default: `metrics`).
- `windows_exporter_telemetry_max_requests` Maximum number of concurrent requests. 0 to disable (default: `5`).
- `windows_exporter_log_file` Output file of log messages. Supported values are: `stdout`, `stderr`, `eventlog` (default), path to log file (example: `C:\Program Files\windows_exporter\exporter.log`).
- `windows_exporter_log_format` A log message format. Supported formats are: `logfmt` (default), `json`.
- `windows_exporter_log_level` The Windows Exporter logging level. Supported levels are: `debug`, `info` (default), `warn`, `error`.
- `windows_exporter_collectors_enabled` Comma-separated list of collectors to use (default: `[defaults]`).
- `windows_exporter_collector` Flags for collectors (default: `''`).
- `windows_exporter_tls_server_config` Certificate and key files for server to use to authenticate to client (default: `{}`).
- `windows_exporter_http_server_config` Enable HTTP/2 support (default: `{}`). Note that HTTP/2 is only supported with TLS.
- `windows_exporter_basic_auth_users` Users and password for basic authentication (default: `{}`). Passwords are automatically hashed with bcrypt.

Dependencies
------------

None.

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
