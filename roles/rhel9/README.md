<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.cis.rhel9
Version: 1.0.0

This role applies the CIS Benchmark hardening steps on RHEL9-based machines.

## Requirements

| Platform | Versions |
| -------- | -------- |
| EL | <ul><li>9</li></ul> |

## Dependencies

| Collection |
| ---------- |
| ansible.posix |
| community.general |

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| rhel9cis_skip_reboot | Whether to skip the reboot step. | bool | no |  | true |
| rhel9cis_level | The CIS benchmark level to apply. | int | no | <ul><li>1</li><li>2</li></ul> | 2 |
| rhel9cis_machine_type | The type of machine for which to apply the CIS benchmarks. | str | no | <ul><li>server</li><li>workstation</li></ul> | server |
| rhel9cis_rule_1_1_1_1_enabled | Whether to apply CIS rule 1.1.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_1_2_enabled | Whether to apply CIS rule 1.1.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_2_1_enabled | Whether to apply CIS rule 1.1.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_2_2_enabled | Whether to apply CIS rule 1.1.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_2_3_enabled | Whether to apply CIS rule 1.1.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_2_4_enabled | Whether to apply CIS rule 1.1.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_3_1_enabled | Whether to apply CIS rule 1.1.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_3_2_enabled | Whether to apply CIS rule 1.1.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_3_3_enabled | Whether to apply CIS rule 1.1.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_4_1_enabled | Whether to apply CIS rule 1.1.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_4_2_enabled | Whether to apply CIS rule 1.1.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_4_3_enabled | Whether to apply CIS rule 1.1.4.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_4_4_enabled | Whether to apply CIS rule 1.1.4.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_5_1_enabled | Whether to apply CIS rule 1.1.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_5_2_enabled | Whether to apply CIS rule 1.1.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_5_3_enabled | Whether to apply CIS rule 1.1.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_5_4_enabled | Whether to apply CIS rule 1.1.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_6_1_enabled | Whether to apply CIS rule 1.1.6.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_6_2_enabled | Whether to apply CIS rule 1.1.6.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_6_3_enabled | Whether to apply CIS rule 1.1.6.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_6_4_enabled | Whether to apply CIS rule 1.1.6.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_7_1_enabled | Whether to apply CIS rule 1.1.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_7_2_enabled | Whether to apply CIS rule 1.1.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_7_3_enabled | Whether to apply CIS rule 1.1.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_8_1_enabled | Whether to apply CIS rule 1.1.8.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_8_2_enabled | Whether to apply CIS rule 1.1.8.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_8_3_enabled | Whether to apply CIS rule 1.1.8.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_8_4_enabled | Whether to apply CIS rule 1.1.8.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_2_1_enabled | Whether to apply CIS rule 1.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_2_2_enabled | Whether to apply CIS rule 1.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_2_3_enabled | Whether to apply CIS rule 1.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_2_4_enabled | Whether to apply CIS rule 1.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_3_1_enabled | Whether to apply CIS rule 1.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_3_2_enabled | Whether to apply CIS rule 1.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_3_3_enabled | Whether to apply CIS rule 1.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_4_1_enabled | Whether to apply CIS rule 1.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_4_2_enabled | Whether to apply CIS rule 1.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_5_1_enabled | Whether to apply CIS rule 1.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_5_2_enabled | Whether to apply CIS rule 1.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_5_3_enabled | Whether to apply CIS rule 1.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_1_enabled | Whether to apply CIS rule 1.6.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_2_enabled | Whether to apply CIS rule 1.6.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_3_enabled | Whether to apply CIS rule 1.6.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_4_enabled | Whether to apply CIS rule 1.6.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_5_enabled | Whether to apply CIS rule 1.6.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_6_enabled | Whether to apply CIS rule 1.6.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_7_enabled | Whether to apply CIS rule 1.6.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_6_1_8_enabled | Whether to apply CIS rule 1.6.1.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_1_enabled | Whether to apply CIS rule 1.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_2_enabled | Whether to apply CIS rule 1.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_3_enabled | Whether to apply CIS rule 1.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_4_enabled | Whether to apply CIS rule 1.7.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_5_enabled | Whether to apply CIS rule 1.7.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_7_6_enabled | Whether to apply CIS rule 1.7.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_1_enabled | Whether to apply CIS rule 1.8.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_2_enabled | Whether to apply CIS rule 1.8.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_3_enabled | Whether to apply CIS rule 1.8.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_4_enabled | Whether to apply CIS rule 1.8.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_5_enabled | Whether to apply CIS rule 1.8.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_6_enabled | Whether to apply CIS rule 1.8.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_7_enabled | Whether to apply CIS rule 1.8.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_8_enabled | Whether to apply CIS rule 1.8.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_9_enabled | Whether to apply CIS rule 1.8.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_8_10_enabled | Whether to apply CIS rule 1.8.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_9_enabled | Whether to apply CIS rule 1.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_10_enabled | Whether to apply CIS rule 1.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_1_1_enabled | Whether to apply CIS rule 2.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_1_2_enabled | Whether to apply CIS rule 2.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_1_enabled | Whether to apply CIS rule 2.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_2_enabled | Whether to apply CIS rule 2.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_3_enabled | Whether to apply CIS rule 2.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_4_enabled | Whether to apply CIS rule 2.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_5_enabled | Whether to apply CIS rule 2.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_6_enabled | Whether to apply CIS rule 2.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_7_enabled | Whether to apply CIS rule 2.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_8_enabled | Whether to apply CIS rule 2.2.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_9_enabled | Whether to apply CIS rule 2.2.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_10_enabled | Whether to apply CIS rule 2.2.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_11_enabled | Whether to apply CIS rule 2.2.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_12_enabled | Whether to apply CIS rule 2.2.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_13_enabled | Whether to apply CIS rule 2.2.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_14_enabled | Whether to apply CIS rule 2.2.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_15_enabled | Whether to apply CIS rule 2.2.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_16_enabled | Whether to apply CIS rule 2.2.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_17_enabled | Whether to apply CIS rule 2.2.17. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_2_18_enabled | Whether to apply CIS rule 2.2.18. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_3_1_enabled | Whether to apply CIS rule 2.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_3_2_enabled | Whether to apply CIS rule 2.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_3_3_enabled | Whether to apply CIS rule 2.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_3_4_enabled | Whether to apply CIS rule 2.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_2_4_enabled | Whether to apply CIS rule 2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_1_1_enabled | Whether to apply CIS rule 3.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_1_2_enabled | Whether to apply CIS rule 3.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_1_3_enabled | Whether to apply CIS rule 3.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_2_1_enabled | Whether to apply CIS rule 3.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_2_2_enabled | Whether to apply CIS rule 3.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_1_enabled | Whether to apply CIS rule 3.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_2_enabled | Whether to apply CIS rule 3.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_3_enabled | Whether to apply CIS rule 3.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_4_enabled | Whether to apply CIS rule 3.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_5_enabled | Whether to apply CIS rule 3.3.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_6_enabled | Whether to apply CIS rule 3.3.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_7_enabled | Whether to apply CIS rule 3.3.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_8_enabled | Whether to apply CIS rule 3.3.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_3_9_enabled | Whether to apply CIS rule 3.3.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_1_1_enabled | Whether to apply CIS rule 3.4.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_1_2_enabled | Whether to apply CIS rule 3.4.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_1_enabled | Whether to apply CIS rule 3.4.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_2_enabled | Whether to apply CIS rule 3.4.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_3_enabled | Whether to apply CIS rule 3.4.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_4_enabled | Whether to apply CIS rule 3.4.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_5_enabled | Whether to apply CIS rule 3.4.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_6_enabled | Whether to apply CIS rule 3.4.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_3_4_2_7_enabled | Whether to apply CIS rule 3.4.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_1_1_enabled | Whether to apply CIS rule 4.1.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_1_2_enabled | Whether to apply CIS rule 4.1.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_1_3_enabled | Whether to apply CIS rule 4.1.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_1_4_enabled | Whether to apply CIS rule 4.1.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_2_1_enabled | Whether to apply CIS rule 4.1.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_2_2_enabled | Whether to apply CIS rule 4.1.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_2_3_enabled | Whether to apply CIS rule 4.1.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_1_enabled | Whether to apply CIS rule 4.1.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_2_enabled | Whether to apply CIS rule 4.1.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_3_enabled | Whether to apply CIS rule 4.1.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_4_enabled | Whether to apply CIS rule 4.1.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_5_enabled | Whether to apply CIS rule 4.1.3.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_6_enabled | Whether to apply CIS rule 4.1.3.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_7_enabled | Whether to apply CIS rule 4.1.3.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_8_enabled | Whether to apply CIS rule 4.1.3.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_9_enabled | Whether to apply CIS rule 4.1.3.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_10_enabled | Whether to apply CIS rule 4.1.3.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_11_enabled | Whether to apply CIS rule 4.1.3.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_12_enabled | Whether to apply CIS rule 4.1.3.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_13_enabled | Whether to apply CIS rule 4.1.3.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_14_enabled | Whether to apply CIS rule 4.1.3.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_15_enabled | Whether to apply CIS rule 4.1.3.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_16_enabled | Whether to apply CIS rule 4.1.3.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_17_enabled | Whether to apply CIS rule 4.1.3.17. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_18_enabled | Whether to apply CIS rule 4.1.3.18. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_19_enabled | Whether to apply CIS rule 4.1.3.19. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_20_enabled | Whether to apply CIS rule 4.1.3.20. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_3_21_enabled | Whether to apply CIS rule 4.1.3.21. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_1_enabled | Whether to apply CIS rule 4.1.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_2_enabled | Whether to apply CIS rule 4.1.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_3_enabled | Whether to apply CIS rule 4.1.4.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_4_enabled | Whether to apply CIS rule 4.1.4.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_5_enabled | Whether to apply CIS rule 4.1.4.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_6_enabled | Whether to apply CIS rule 4.1.4.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_7_enabled | Whether to apply CIS rule 4.1.4.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_8_enabled | Whether to apply CIS rule 4.1.4.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_9_enabled | Whether to apply CIS rule 4.1.4.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_1_4_10_enabled | Whether to apply CIS rule 4.1.4.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_1_enabled | Whether to apply CIS rule 4.2.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_2_enabled | Whether to apply CIS rule 4.2.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_3_enabled | Whether to apply CIS rule 4.2.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_4_enabled | Whether to apply CIS rule 4.2.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_5_enabled | Whether to apply CIS rule 4.2.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_6_enabled | Whether to apply CIS rule 4.2.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_1_7_enabled | Whether to apply CIS rule 4.2.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_1_1_enabled | Whether to apply CIS rule 4.2.2.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_1_2_enabled | Whether to apply CIS rule 4.2.2.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_1_3_enabled | Whether to apply CIS rule 4.2.2.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_1_4_enabled | Whether to apply CIS rule 4.2.2.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_2_enabled | Whether to apply CIS rule 4.2.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_3_enabled | Whether to apply CIS rule 4.2.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_4_enabled | Whether to apply CIS rule 4.2.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_5_enabled | Whether to apply CIS rule 4.2.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_6_enabled | Whether to apply CIS rule 4.2.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_2_7_enabled | Whether to apply CIS rule 4.2.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_2_3_enabled | Whether to apply CIS rule 4.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_4_3_enabled | Whether to apply CIS rule 4.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_1_enabled | Whether to apply CIS rule 5.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_2_enabled | Whether to apply CIS rule 5.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_3_enabled | Whether to apply CIS rule 5.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_4_enabled | Whether to apply CIS rule 5.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_5_enabled | Whether to apply CIS rule 5.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_6_enabled | Whether to apply CIS rule 5.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_7_enabled | Whether to apply CIS rule 5.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_8_enabled | Whether to apply CIS rule 5.1.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_1_9_enabled | Whether to apply CIS rule 5.1.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_1_enabled | Whether to apply CIS rule 5.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_2_enabled | Whether to apply CIS rule 5.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_3_enabled | Whether to apply CIS rule 5.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_4_enabled | Whether to apply CIS rule 5.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_5_enabled | Whether to apply CIS rule 5.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_6_enabled | Whether to apply CIS rule 5.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_7_enabled | Whether to apply CIS rule 5.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_8_enabled | Whether to apply CIS rule 5.2.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_9_enabled | Whether to apply CIS rule 5.2.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_10_enabled | Whether to apply CIS rule 5.2.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_11_enabled | Whether to apply CIS rule 5.2.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_12_enabled | Whether to apply CIS rule 5.2.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_13_enabled | Whether to apply CIS rule 5.2.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_14_enabled | Whether to apply CIS rule 5.2.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_15_enabled | Whether to apply CIS rule 5.2.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_16_enabled | Whether to apply CIS rule 5.2.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_17_enabled | Whether to apply CIS rule 5.2.17. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_18_enabled | Whether to apply CIS rule 5.2.18. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_19_enabled | Whether to apply CIS rule 5.2.19. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_2_20_enabled | Whether to apply CIS rule 5.2.20. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_1_enabled | Whether to apply CIS rule 5.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_2_enabled | Whether to apply CIS rule 5.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_3_enabled | Whether to apply CIS rule 5.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_4_enabled | Whether to apply CIS rule 5.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_5_enabled | Whether to apply CIS rule 5.3.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_6_enabled | Whether to apply CIS rule 5.3.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_3_7_enabled | Whether to apply CIS rule 5.3.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_4_1_enabled | Whether to apply CIS rule 5.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_4_2_enabled | Whether to apply CIS rule 5.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_5_1_enabled | Whether to apply CIS rule 5.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_5_2_enabled | Whether to apply CIS rule 5.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_5_3_enabled | Whether to apply CIS rule 5.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_5_4_enabled | Whether to apply CIS rule 5.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_1_1_enabled | Whether to apply CIS rule 5.6.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_1_2_enabled | Whether to apply CIS rule 5.6.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_1_3_enabled | Whether to apply CIS rule 5.6.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_1_4_enabled | Whether to apply CIS rule 5.6.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_1_5_enabled | Whether to apply CIS rule 5.6.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_2_enabled | Whether to apply CIS rule 5.6.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_3_enabled | Whether to apply CIS rule 5.6.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_4_enabled | Whether to apply CIS rule 5.6.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_5_enabled | Whether to apply CIS rule 5.6.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_5_6_6_enabled | Whether to apply CIS rule 5.6.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_1_enabled | Whether to apply CIS rule 6.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_2_enabled | Whether to apply CIS rule 6.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_3_enabled | Whether to apply CIS rule 6.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_4_enabled | Whether to apply CIS rule 6.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_5_enabled | Whether to apply CIS rule 6.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_6_enabled | Whether to apply CIS rule 6.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_7_enabled | Whether to apply CIS rule 6.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_8_enabled | Whether to apply CIS rule 6.1.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_9_enabled | Whether to apply CIS rule 6.1.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_10_enabled | Whether to apply CIS rule 6.1.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_11_enabled | Whether to apply CIS rule 6.1.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_12_enabled | Whether to apply CIS rule 6.1.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_13_enabled | Whether to apply CIS rule 6.1.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_14_enabled | Whether to apply CIS rule 6.1.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_1_15_enabled | Whether to apply CIS rule 6.1.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_1_enabled | Whether to apply CIS rule 6.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_2_enabled | Whether to apply CIS rule 6.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_3_enabled | Whether to apply CIS rule 6.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_4_enabled | Whether to apply CIS rule 6.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_5_enabled | Whether to apply CIS rule 6.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_6_enabled | Whether to apply CIS rule 6.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_7_enabled | Whether to apply CIS rule 6.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_8_enabled | Whether to apply CIS rule 6.2.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_9_enabled | Whether to apply CIS rule 6.2.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_10_enabled | Whether to apply CIS rule 6.2.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_11_enabled | Whether to apply CIS rule 6.2.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_12_enabled | Whether to apply CIS rule 6.2.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_13_enabled | Whether to apply CIS rule 6.2.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_14_enabled | Whether to apply CIS rule 6.2.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_15_enabled | Whether to apply CIS rule 6.2.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_6_2_16_enabled | Whether to apply CIS rule 6.2.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| rhel9cis_rule_1_1_1_1_force | Whether to override the level requirement for CIS rule 1.1.1.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_1_2_force | Whether to override the level requirement for CIS rule 1.1.1.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_3_1_force | Whether to override the level requirement for CIS rule 1.1.3.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_4_1_force | Whether to override the level requirement for CIS rule 1.1.4.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_5_1_force | Whether to override the level requirement for CIS rule 1.1.5.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_6_1_force | Whether to override the level requirement for CIS rule 1.1.6.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_1_7_1_force | Whether to override the level requirement for CIS rule 1.1.7.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_2_4_force | Whether to override the level requirement for CIS rule 1.2.4. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_6_1_5_force | Whether to override the level requirement for CIS rule 1.6.1.5. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_8_1_force | Whether to override the level requirement for CIS rule 1.8.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_8_6_force | Whether to override the level requirement for CIS rule 1.8.6. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_1_8_7_force | Whether to override the level requirement for CIS rule 1.8.7. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_2_2_1_force | Whether to override the level requirement for CIS rule 2.2.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_2_2_2_force | Whether to override the level requirement for CIS rule 2.2.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_3_1_3_force | Whether to override the level requirement for CIS rule 3.1.3. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_1_1_force | Whether to override the level requirement for CIS rule 4.1.1.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_1_2_force | Whether to override the level requirement for CIS rule 4.1.1.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_1_3_force | Whether to override the level requirement for CIS rule 4.1.1.3. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_1_4_force | Whether to override the level requirement for CIS rule 4.1.1.4. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_2_1_force | Whether to override the level requirement for CIS rule 4.1.2.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_2_2_force | Whether to override the level requirement for CIS rule 4.1.2.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_2_3_force | Whether to override the level requirement for CIS rule 4.1.2.3. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_1_force | Whether to override the level requirement for CIS rule 4.1.3.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_2_force | Whether to override the level requirement for CIS rule 4.1.3.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_3_force | Whether to override the level requirement for CIS rule 4.1.3.3. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_4_force | Whether to override the level requirement for CIS rule 4.1.3.4. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_5_force | Whether to override the level requirement for CIS rule 4.1.3.5. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_6_force | Whether to override the level requirement for CIS rule 4.1.3.6. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_7_force | Whether to override the level requirement for CIS rule 4.1.3.7. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_8_force | Whether to override the level requirement for CIS rule 4.1.3.8. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_9_force | Whether to override the level requirement for CIS rule 4.1.3.9. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_10_force | Whether to override the level requirement for CIS rule 4.1.3.10. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_11_force | Whether to override the level requirement for CIS rule 4.1.3.11. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_12_force | Whether to override the level requirement for CIS rule 4.1.3.12. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_13_force | Whether to override the level requirement for CIS rule 4.1.3.13. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_14_force | Whether to override the level requirement for CIS rule 4.1.3.14. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_15_force | Whether to override the level requirement for CIS rule 4.1.3.15. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_16_force | Whether to override the level requirement for CIS rule 4.1.3.16. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_17_force | Whether to override the level requirement for CIS rule 4.1.3.17. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_18_force | Whether to override the level requirement for CIS rule 4.1.3.18. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_19_force | Whether to override the level requirement for CIS rule 4.1.3.19. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_20_force | Whether to override the level requirement for CIS rule 4.1.3.20. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_3_21_force | Whether to override the level requirement for CIS rule 4.1.3.21. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_1_force | Whether to override the level requirement for CIS rule 4.1.4.1. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_2_force | Whether to override the level requirement for CIS rule 4.1.4.2. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_3_force | Whether to override the level requirement for CIS rule 4.1.4.3. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_4_force | Whether to override the level requirement for CIS rule 4.1.4.4. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_5_force | Whether to override the level requirement for CIS rule 4.1.4.5. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_6_force | Whether to override the level requirement for CIS rule 4.1.4.6. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_7_force | Whether to override the level requirement for CIS rule 4.1.4.7. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_8_force | Whether to override the level requirement for CIS rule 4.1.4.8. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_9_force | Whether to override the level requirement for CIS rule 4.1.4.9. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_4_1_4_10_force | Whether to override the level requirement for CIS rule 4.1.4.10. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_5_2_12_force | Whether to override the level requirement for CIS rule 5.2.12. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_5_2_13_force | Whether to override the level requirement for CIS rule 5.2.13. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_rule_6_1_15_force | Whether to override the level requirement for CIS rule 6.1.15. This applies when the machine type is appropriate. | bool | no |  | false |
| rhel9cis_tmp_mount_opts | The mount options for the /tmp partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid", "noexec"] |
| rhel9cis_var_mount_opts | The mount options for the /var partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid"] |
| rhel9cis_var_tmp_mount_opts | The mount options for the /var/tmp partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid", "noexec"] |
| rhel9cis_var_log_mount_opts | The mount options for the /var/log partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid", "noexec"] |
| rhel9cis_var_log_audit_mount_opts | The mount options for the /var/log/audit partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid", "noexec"] |
| rhel9cis_home_mount_opts | The mount options for the /home partition. | list of 'str' | no |  | ["defaults", "nodev", "nosuid"] |
| rhel9cis_dev_shm_mount_opts | The mount options for the /dev/shm partition. | list of 'str' | no |  | ["mode=1777", "strictatime", "nodev", "nosuid", "noexec"] |
| rhel9cis_aide_cron_file | The file to use for the AIDE cron job. | path | no |  | /etc/cron.d/aide |
| rhel9cis_aide_cron_hour | The hour to run the AIDE cron job. | int | no |  | 5 |
| rhel9cis_aide_cron_minute | The minute to run the AIDE cron job. | int | no |  | 0 |
| rhel9cis_force_reset_bootloader_password | Whether to force a reset of the bootloader password, even if one is set. Setting this to `true` will make the role not idempotent. | bool | no |  | false |
| rhel9cis_bootloader_password | The bootloader password to set. | str | no |  |  |
| rhel9cis_selinux_policy | The SELinux policy to use. | str | no |  | targeted |
| rhel9cis_selinux_mode | The SELinux mode to use. | str | no |  | enforcing |
| rhel9cis_use_motd | Whether to use the Message of the Day (MOTD). | bool | no |  | true |
| rhel9cis_motd_banner | The banner to use for the Message of the Day (MOTD). | str | no |  | Authorized users only.\n\nAll activity may be monitored and reported.\n\n |
| rhel9cis_use_issue | Whether to use the issue file. | bool | no |  | false |
| rhel9cis_issue_banner | The banner to use for the issue file. | str | no |  | Authorized users only.\n\nAll activity may be monitored and reported.\n\n |
| rhel9cis_use_issue_net | Whether to use the issue.net file. | bool | no |  | false |
| rhel9cis_issue_net_banner | The banner to use for the issue.net file. | str | no |  | Authorized users only.\n\nAll activity may be monitored and reported.\n\n |
| rhel9cis_crypto_policy | The crypto policy to use. | str | no | <ul><li>DEFAULT</li><li>FUTURE</li><li>FIPS</li></ul> | DEFAULT |
| rhel9cis_crypto_subpolicies | The crypto subpolicies to use. | list of 'str' | no |  |  |
| rhel9cis_chrony_servers | The NTP server configuration to use with chrony. | list of dicts of 'rhel9cis_chrony_servers' options | no |  | [{"name": "0.pool.ntp.org", "options": ["minpoll 8"]}, {"name": "1.pool.ntp.org", "options": ["minpoll 8"]}, {"name": "2.pool.ntp.org", "options": ["minpoll 8"]}, {"name": "3.pool.ntp.org", "options": ["minpoll 8"]}] |
| rhel9cis_xorg_needed | Whether the `xorg` package is needed. If set to `true`, the `xorg` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_avahi_needed | Whether the `avahi` package is needed. If set to `true`, the `avahi` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_cups_needed | Whether the `cups` package is needed. If set to `true`, the `cups` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_dhcp_server_needed | Whether the `dhcp-server` package is needed. If set to `true`, the `dhcp-server` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_bind_needed | Whether the `bind` package is needed. If set to `true`, the `bind` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_vsftpd_needed | Whether the `vsftpd` package is needed. If set to `true`, the `vsftpd` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_tftp_server_needed | Whether the `tftp-server` package is needed. If set to `true`, the `tftp-server` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_httpd_needed | Whether the `httpd` package is needed. If set to `true`, the `httpd` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_nginx_needed | Whether the `nginx` package is needed. If set to `true`, the `nginx` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_dovecot_needed | Whether the `dovecot` package is needed. If set to `true`, the `dovecot` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_cyrus_imapd_needed | Whether the `cyrus-imapd` package is needed. If set to `true`, the `cyrus-imapd` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_samba_needed | Whether the `samba` package is needed. If set to `true`, the `samba` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_squid_needed | Whether the `squid` package is needed. If set to `true`, the `squid` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_net_snmp_needed | Whether the `net-snmp` package is needed. If set to `true`, the `net-snmp` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_telnet_server_needed | Whether the `telnet-server` package is needed. If set to `true`, the `telnet-server` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_dnsmasq_needed | Whether the `dnsmasq` package is needed. If set to `true`, the `dnsmasq` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_postfix_needed | Whether the `postfix` package is needed. If set to `true`, the `postfix` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_nfs_utils_needed | Whether the `nfs-utils` package is needed. If set to `true`, the `nfs-utils` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_rpcbind_needed | Whether the `rpcbind` package is needed. If set to `true`, the `rpcbind` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_rsync_daemon_needed | Whether the `rsync-daemon` package is needed. If set to `true`, the `rsync-daemon` package will be remain installed and the services will be disabled instead. | bool | no |  | false |
| rhel9cis_ipv6_needed | Whether IPv6 is needed. | bool | no |  | false |
| rhel9cis_firewall | The firewall to use. | str | no | <ul><li>firewalld</li></ul> | firewalld |
| rhel9cis_firewalld_default_zone | The default zone for firewalld. | str | no |  | public |
| rhel9cis_auditd_backlog_limit | The audit backlog limit. | int | no |  | 8192 |
| rhel9cis_auditd_max_log_file | The maximum auditd log file size. | int | no |  | 10 |
| rhel9cis_auditd_disk_full_action | The action to take when the auditd disk is full. | str | no | <ul><li>single</li><li>halt</li></ul> | halt |
| rhel9cis_auditd_disk_error_action | The action to take when the auditd disk has an error. | str | no | <ul><li>single</li><li>halt</li><li>syslog</li></ul> | halt |
| rhel9cis_syslog | The syslog configuration. | str | no | <ul><li>rsyslog</li><li>journald</li></ul> | rsyslog |
| rhel9cis_remote_log_server | The remote log server to use. | str | no |  | logserver.example.com |
| rhel9cis_journal_server_key_file | The journal server key file. | path | no |  | /etc/ssl/private/journal-upload.pem |
| rhel9cis_journal_server_cert_file | The journal server certificate file. | path | no |  | /etc/ssl/certs/journal-upload.pem |
| rhel9cis_journal_server_trusted_cert_file | The journal server trusted certificate file. | path | no |  | /etc/ssl/ca/trusted.pem |
| rhel9cis_journald_systemmaxuse | The maximum disk usage for the system journal. | str | no |  | 10M |
| rhel9cis_journald_systemkeepfree | The minimum disk space to keep free for the system journal. | str | no |  | 100G |
| rhel9cis_journald_runtimemaxuse | The maximum disk usage for the runtime journal. | str | no |  | 10M |
| rhel9cis_journald_runtimekeepfree | The minimum disk space to keep free for the runtime journal. | str | no |  | 100G |
| rhel9cis_journald_maxfilesec | The maximum file retention time. | str | no |  | 1month |
| rhel9cis_logrotate_frequency | The logrotate frequency. | str | no | <ul><li>daily</li><li>weekly</li><li>monthly</li></ul> | daily |
| rhel9cis_sshd_allow_users | The users to allow for SSH. | list of 'str' | no |  |  |
| rhel9cis_sshd_allow_groups | The groups to allow for SSH. | list of 'str' | no |  | ["wheel"] |
| rhel9cis_sshd_deny_users | The users to deny for SSH. | list of 'str' | no |  |  |
| rhel9cis_sshd_deny_groups | The groups to deny for SSH. | list of 'str' | no |  |  |
| rhel9cis_sshd_log_level | The log level for SSH. | str | no | <ul><li>INFO</li><li>VERBOSE</li></ul> | INFO |
| rhel9cis_sshd_max_auth_tries | The maximum number of authentication attempts. | int | no |  | 4 |
| rhel9cis_sshd_max_startups_before_dropping | The maximum number of startups before dropping. | int | no |  | 10 |
| rhel9cis_sshd_max_startups_drop_percentage | The maximum percentage of startups to drop. | int | no |  | 30 |
| rhel9cis_sshd_max_startups_absolute_maximum | The absolute maximum number of startups. | int | no |  | 60 |
| rhel9cis_sshd_max_sessions | The maximum number of sessions. | int | no |  | 10 |
| rhel9cis_sshd_login_grace_time | The login grace time in seconds. | int | no |  | 60 |
| rhel9cis_sshd_client_alive_interval | The interval for the client alive messages in seconds. | int | no |  | 15 |
| rhel9cis_sshd_client_alive_count_max | The maximum number of client alive messages. | int | no |  | 3 |
| rhel9cis_sudo_log_file | The log file for sudo. | path | no |  | /var/log/sudo.log |
| rhel9cis_sudo_authentication_timeout | The authentication timeout for sudo in seconds. | int | no |  | 15 |
| rhel9cis_su_group_name | The group name for the su command. | str | no |  | su |
| rhel9cis_su_group_members | The group members for the su command. | list of 'str' | no |  | ["root"] |
| rhel9cis_password_min_length | The minimum length for a new password. | int | no |  | 14 |
| rhel9cis_lockout_failed_attempts | The number of failed login attempts before lockout. | int | no |  | 5 |
| rhel9cis_lockout_unlock_time | The time in seconds to unlock the account. | int | no |  | 900 |
| rhel9cis_passwords_remembered | The number of passwords remembered. | int | no |  | 24 |
| rhel9cis_password_hashing_algorithm | The password hashing algorithm to use. | str | no | <ul><li>sha512</li><li>yescrypt</li></ul> | sha512 |
| rhel9cis_password_expiration_days | The number of days before password expiration. | int | no |  | 365 |
| rhel9cis_min_password_age | The minimum password age in days before it can be changed. | int | no |  | 1 |
| rhel9cis_password_expiration_warning_days | The number of days before password expiration warning. | int | no |  | 7 |
| rhel9cis_inactive_password_lock_days | The number of days before inactive password lock. | int | no |  | 30 |
| rhel9cis_shell_timeout | The shell timeout in seconds. | int | no |  | 900 |

### Options for rhel9cis_chrony_servers
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| name | The NTP server name. | str | yes |  |  |
| options | The NTP server options. | list of 'str' | no |  |  |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
