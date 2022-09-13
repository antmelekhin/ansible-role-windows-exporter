Windows Exporter
================

Ansible роль для установки, настройки и обновления [Windows Exporter](https://github.com/prometheus-community/windows_exporter).

Требования
----------

- Поддерживаемая версия Ansible: 2.7 и выше.
- `pywinrm` для подключения [Ansible через WinRM](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html) (для Windows).
- Список поддерживаемых платформ описан в файле метаданных роли.

Используемые переменные
-----------------------

- `windows_exporter_version` Версия Windows Exporter для установки (default: `0.18.1`).
- `windows_exporter_package_name` Имя пакета.
- `windows_exporter_download_url` Ссылка на скачивание архива с приложением.
- `windows_exporter_listen_address` Адрес сервера с метриками (default: `0.0.0.0`).
- `windows_exporter_listen_port` Порт сервера с метриками (default: `9182`).
- `windows_exporter_metrics_path` Путь до метрик (default: `metrics`).
- `windows_exporter_log_level` Уровень логирования экспортера (default: `debug`).
- `windows_exporter_collectors_enabled` Включенные коллекторы (default: `[defaults]`).
- `windows_exporter_collector` Настраиваемый фильтр для метрик (default: `''`).

Зависимости
-----------

Отсутствуют.

Пример использования
--------------------

- Настраиваем Windows Exporter, дополнительно к дефолтным коллекторам добавляем коллетор memory и настраиваем сбор метрик коллектора service только для сервиса windows_exporter.

  ```yaml
  ---
  - name: 'Setup Windows Exporter'
    hosts: windows_exporter

    roles:
      - role: 'ansible-role-windows-exporter'
        windows_exporter_collectors_enabled: '[defaults],memory'
        windows_exporter_collector:
          - name: service
            flags:
              services-where: Name='windows_exporter'
  ```

Лицензия
--------

MIT

Информация об авторе
--------------------

Мелехин Антон
