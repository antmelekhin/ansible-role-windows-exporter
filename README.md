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

- `windows_exporter__version` Версия Windows Exporter для установки (default: `0.18.1`).
- `windows_exporter__architecture` Архитектура Windows Exporter (default: `amd64`).
- `windows_exporter__download_url` Ссылка на скачивание архива с приложением.
- `windows_exporter__listen_address` Адрес сервера с метриками (default: `0.0.0.0`).
- `windows_exporter__listen_port` Порт сервера с метриками (default: `9182`).
- `windows_exporter__metrics_path` Путь до метрик (default: `metrics`).
- `windows_exporter__log_level` Уровень логирования экспортера (default: `debug`).
- `windows_exporter__enabled_collectors` Включенные коллекторы (default: `[defaults]`).
- `windows_exporter__collector` Настраиваемый фильтр для метрик (default: `''`).

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
        windows_exporter__enabled_collectors: '[defaults],memory'
        windows_exporter__collector:
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
