# Changelog

## [1.2.7](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.6...v1.2.7) (2024-03-08)


### Fixes

* delegate to localhost download binary ([#14](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/14)) ([2aa18f7](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/2aa18f71ea8ae970ac1570af9137aef1a41ecddb))

## [1.2.6](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.5...v1.2.6) (2024-03-08)


### Fixes

* **version:** windows_exporter updated to `0.25.1` release ([#12](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/12)) ([977c445](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/977c4452692cf0d58bb3e41612937f150fdbce60))

## [1.2.5](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.4...v1.2.5) (2024-03-08)


### Continuous Integration

* fix publish workflow ([049d24d](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/049d24d3d32f0d1702a5d2792889679e4aad2d52))


### Fixes

* **version:** windows_exporter updated to `0.25.0` release ([#11](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/11)) ([fdf5c61](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/fdf5c61df5366430fd1844adc25a08b7b80f96c6))


### Styles

* update repo description ([38940e2](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/38940e2c0f880d2da65ee62ef4b56c31053f571f))
* update task names ([d8a6e60](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/d8a6e604f86f16d86bd66de3058ff5225b50a017))
* use double underlined register variable ([0eb3938](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/0eb3938357802a8328b4a9572a40c952f788e013))

## [1.2.4](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.3...v1.2.4) (2023-10-09)


### Fixes

* correct `win_stat` module fqcn ([#9](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/9)) ([1b2d394](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/1b2d394b524bdd4ba00a32ec6dde7ad31971fc3d))


### Tests

* **fix:** set `role_name_check` as skip_list and add this key in `tls-and-basic-auth` scenario ([#8](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/8)) ([ade622a](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/ade622a0dee38a939b2460852502daa27cb12898))

## [1.2.3](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.2...v1.2.3) (2023-10-05)


### Fixes

* **version:** windows_exporter updated to `0.24.0` release ([#6](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/6)) ([eb87e30](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/eb87e3074e207285bd0a62e1ee45456ba88268d5))

## [1.2.2](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.1...v1.2.2) (2023-09-23)


### Fixes

* replaced listen-address option from telemetry to web ([#5](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/5)) ([24d6423](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/24d6423777089bcd542727af33a7c75708f4677e))

## [1.2.1](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.0...v1.2.1) (2023-08-22)


### Fixes

* add fqcn for all modules ([b49a59f](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/b49a59f2730b0cefa9a7f550a3c321dcb5efffaf))

## [1.2.0](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.1.3...v1.2.0) (2023-08-22)


### Features

* add missing config values ([cb1c15e](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/cb1c15e2bb62b93afb359d7139ebb0714e040f8b))

## [1.1.3](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.1.2...v1.1.3) (2023-07-28)


### Fixes

* **version:** windows_exporter updated to `0.23.1` release ([#3](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/3)) ([0d0490c](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/0d0490c6f4be593a3bc91940f141f07dcae21ab3))

## [1.1.2](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.1.1...v1.1.2) (2023-07-03)


### Fixes

* update `_windows_exporter_arguments` variable ([3cfbf77](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/3cfbf778a1ed15e0ab76f7823e82ffe981a12f01))


### Styles

* add quotes in notify name ([eb4fa27](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/eb4fa274c372c6086f673ee5fa903d2af40a2fba))

## [1.1.1](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.1.0...v1.1.1) (2023-07-01)


### Fixes

* **version:** windows_exporter updated to `0.22.0` release ([f157604](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/f157604a821af480b102003ffce513e153e0bd2d))

## [1.1.0](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.0.1...v1.1.0) (2023-06-26)


### Code Refactoring

* update variables ([aad8813](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/aad881338c50f10f48d93dfa486a5f9eeef9b0f8))


### Features

* add configuration for tls and basic auth ([bc07a8a](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/bc07a8af6cafef14f35a09cc9b00f8ec53df08e8))

## [1.0.1](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.0.0...v1.0.1) (2023-06-23)


### Continuous Integration

* add `publish` and `release` workflows ([fe7e739](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/fe7e739e144258ca911affa786baff1aa988f9c7))
* add `update-version` script and workflow ([49753a1](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/49753a1aaac58ffa85e96ee69d7e1765ad083ac6))


### Documentation

* update README and meta ([ab228d8](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/ab228d8fc210d3d15f81a4cd4cc83d5f1c508cac))


### Fixes

* reordering key names ([fafe834](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/fafe83418713f79bb699d7816ee439ebb7c0d065))
* update version condition for installation task block ([f1cdbb9](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/f1cdbb9d7ded82f5238c24186bc9d3ae2a8ea0b3))


### Tests

* add `.ansible-lint` file and minor fixes molecule ([135259a](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/135259a65abb02f0deb02a6bd1155b13c6458fd7))
