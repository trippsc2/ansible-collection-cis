# Changelog

All notable changes to this project will be documented in this file.

## [1.2.1] - 2025-01-08

- Added Changelog.
- Updated collection README documentation.

## [1.2.0] - 2024-11-20

- *trippsc2.cis.rhel8* role - Updated role to be based on CIS Benchmarks v2.0.0. See the CIS Benchmark document for details.
- *trippsc2.cis.rhel8* role - Split `rhel8cis_mount_with_uuid` variable into `rhel8cis_home_mount_with_uuid`, `rhel8cis_var_mount_with_uuid`, `rhel8cis_var_log_mount_with_uuid`, `rhel8cis_var_log_audit_mount_with_uuid`, and `rhel8cis_var_tmp_mount_with_uuid` variables to allow UUID mounting to be used on a per mount point basis.
- *trippsc2.cis.rhel9* role - Updated role to be based on CIS Benchmarks v2.0.0. See the CIS Benchmark document for details.
- *trippsc2.cis.rhel9* role - Split `rhel9cis_mount_with_uuid` variable into `rhel9cis_home_mount_with_uuid`, `rhel9cis_var_mount_with_uuid`, `rhel9cis_var_log_mount_with_uuid`, `rhel9cis_var_log_audit_mount_with_uuid`, and `rhel9cis_var_tmp_mount_with_uuid` variables to allow UUID mounting to be used on a per mount point basis.
- *trippsc2.cis.windows2019* role - Updated role to be based on CIS Benchmarks v3.0.1. See the CIS Benchmark document for details.
- *trippsc2.cis.windows2022* role - Updated role to be based on CIS Benchmarks v3.0.0. See the CIS Benchmark document for details.

## [1.1.1] - 2024-10-22

- *trippsc2.cis.windows2019* role - Removed `os_family` subset for fact gathering step as it is not used on Windows machines.
- *trippsc2.cis.windows2022* role - Removed `os_family` subset for fact gathering step as it is not used on Windows machines.

## [1.1.0] - 2024-09-26

- *trippsc2.cis.rhel8* role - Added `rhel8cis_mount_with_uuid` option (enabled by default) to mount using UUIDs instead of device paths.
- *trippsc2.cis.rhel9* role - Added `rhel9cis_mount_with_uuid` option (enabled by default) to mount using UUIDs instead of device paths.

## [1.0.9] - 2024-09-10

- *trippsc2.cis.rhel9* role - Added missing variable `rhel9cis_rule_2_3_2_force`.

## [1.0.8] - 2024-09-06

- *trippsc2.cis.rhel8* role - Added `rhel8cis_bootloader_password` variable with `no_log` option to allow for setting the bootloader password.
- *trippsc2.cis.rhel9* role - Added `no_log` option to `rhel9cis_bootloader_password` variable.

## [1.0.7] - 2024-08-09

- Minimum Ansible version changed from `2.14` to `2.15` due to EOL status.

## [1.0.6] - 2024-07-08

- Updated manifest file to ensure that molecule tests are not included in releases.

## [1.0.5] - 2024-06-30

- *trippsc2.cis.windows2019* role - Fixed variables that did not match the role argument spec when used in the role.

## [1.0.4] - 2024-06-30

- *trippsc2.cis.windows2019* role - Renamed `w2022cis_login_message_text` and `w2022cis_login_message_title` variables to `w2019cis_login_message_text` and `w2019cis_login_message_title` variables to match the naming scheme.

## [1.0.3] - 2024-06-30

- *trippsc2.cis.windows2019* role - Renamed `w2019cis_legal_notice_text` and `w2019cis_legal_notice_title` variables to `w2022cis_login_message_text` and `w2022cis_login_message_title` variables. The name prefixes are fixed in v1.0.4.
- *trippsc2.cis.windows2022* role - Renamed `w2022cis_legal_notice_text` and `w2022cis_legal_notice_title` variables to `w2022cis_login_message_text` and `w2022cis_login_message_title` variables.

## [1.0.2] - 2024-06-20

- *trippsc2.cis.rhel8* role - Updated documentation and role metadata for readability.
- *trippsc2.cis.rhel9* role - Updated documentation and role metadata for readability.
- *trippsc2.cis.windows2019* role - Updated documentation and role metadata for readability.
- *trippsc2.cis.windows2022* role - Updated documentation and role metadata for readability.

## [1.0.1] - 2024-06-20

- *trippsc2.cis.rhel8* role - Removed validation that is handled by role argument spec.
- *trippsc2.cis.rhel9* role - Removed validation that is handled by role argument spec.
- *trippsc2.cis.windows2019* role - Removed validation that is handled by role argument spec.
- *trippsc2.cis.windows2022* role - Removed validation that is handled by role argument spec.

## [1.0.0] - 2024-06-13

- Initial release.
- *trippsc2.cis.rhel8* role - Role added.
- *trippsc2.cis.rhel9* role - Role added.
- *trippsc2.cis.windows2019* role - Role added.
- *trippsc2.cis.windows2022* role - Role added.
