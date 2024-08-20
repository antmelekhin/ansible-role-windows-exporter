# Changelog

## [3.0.2](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v3.0.1...v3.0.2) (2024-08-20)


### Fixes

* **version:** windows_exporter updated to `0.27.2` release ([#23](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/23)) ([344d0b1](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/344d0b11ab63d90c771754147b34af539e56d6f9))

## [3.0.1](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v3.0.0...v3.0.1) (2024-08-13)


### Fixes

* **version:** windows_exporter updated to `0.27.0` release ([#22](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/22)) ([889263b](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/889263ba928f41fdc51184c1f83e9724120f6ae0))

## [3.0.0](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v2.1.0...v3.0.0) (2024-08-09)


### ⚠ BREAKING CHANGES

* rename `windows_exporter_collector` variable (#21)

### Fixes

* rename `windows_exporter_collector` variable ([#21](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/21)) ([e2310e9](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/e2310e98c80cf7f6ba688f3d69cfedc7c5d8469f))

## [2.1.0](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v2.0.3...v2.1.0) (2024-08-09)


### Features

* add `meta/argument_specs.yml` file and another improvements ([#19](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/19)) ([262cd99](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/262cd99b26943588e4d1aa53af436999b9912304))

## [2.0.3](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v2.0.2...v2.0.3) (2024-08-06)


### Fixes

* **version:** windows_exporter updated to `0.26.2` release ([#20](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/20)) ([456f2d7](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/456f2d7c947b766c9501a2de966275612cb34635))

## [2.0.2](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v2.0.1...v2.0.2) (2024-07-31)


### Fixes

* **version:** windows_exporter updated to `0.26.0` release ([#18](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/18)) ([bc042e7](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/bc042e74949004fa7660b14228d23b7a2e6d3e4c))

## [2.0.1](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v2.0.0...v2.0.1) (2024-07-17)


### Fixes

* add `windows_exporter_checksum_url` variable ([306b927](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/306b927dfa3f939800a417c7cdab9d6231027c91))


### Tests

* clean version output in the `default` scenario ([b0c8361](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/b0c836191e8d791427fd72c5672aba5097fe6b4e))

## [2.0.0](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.8...v2.0.0) (2024-06-06)


### ⚠ BREAKING CHANGES

* update variables and common role style (#17)

### Improvements

* update variables and common role style ([#17](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/17)) ([8231dd7](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/8231dd7db61648879ddfaedf4e4e6e7c1a0ac594))

## [1.2.8](https://github.com/antmelekhin/ansible-role-windows-exporter/compare/v1.2.7...v1.2.8) (2024-05-02)


### Continuous Integration

* add semantic version validation ([7c20d92](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/7c20d920027714f85b33aea9d4f2f1ac3f49fbc0))
* update workflows and release rules ([#15](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/15)) ([da4424e](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/da4424e76a831f2d2fa78348bbdc0c91f0464e7f))


### Documentation

* **README:** fixed examples view for Ansible Galaxy ([d69eaf6](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/d69eaf67d0d95fefea375b5a0821aac6f016cf9d))


### Styles

* add newline to end of file ([1ec0aa8](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/1ec0aa8e8aad0cdbb3767ca009cdbca734b9d30a))
* quote strings and use double underline register variables ([#16](https://github.com/antmelekhin/ansible-role-windows-exporter/issues/16)) ([732e0f3](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/732e0f32f82b6fb21ee2f938cb337690cbc16fc7))
* trim trailing whitespace ([a7cb346](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/a7cb3462913339995eb5bb26c897142a1066d5d5))


### Tests

* rm lint from molecule ([774414e](https://github.com/antmelekhin/ansible-role-windows-exporter/commit/774414eb84ef70c07fdd6204dac14a8a1f300661))

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
