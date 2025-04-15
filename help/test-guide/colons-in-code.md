---
title: Colons in code blocks not rendering
description: UGP-12963 colons in code blocks not rendering
exl-id: 1da12181-f1a2-45e0-9184-1375f3a23bd2
---
# Colonic issues

ACP2E-3096

* _ACP2E-3096_: Incorrect curl headers making `newrelic:create:deploy-marker` not working
  * _Fix note_: The system now correctly formats curl headers, allowing the `newrelic:create:deploy-marker` command to successfully create a deployment marker in New Relic. Previously, incorrect curl headers prevented the creation of a deployment marker in New Relic.
  * More

AC-11999 (no backticks)

* _AC-11999_: dev:di:info error in magento 2.4.7
  * _Fix note_: The system now correctly displays constructor parameters when executing the dev:di:info command, preventing any errors from occurring. Previously, executing this command resulted in an error due to a type mismatch in the argument.
  * _GitHub issue_: <https://github.com/magento/magento2/issues/38740>
  * _GitHub code contribution_: <https://github.com/magento/magento2/commit/0c53bbf7>

AC-11999 (yes backticks)

* _AC-11999_: `dev:di:info` error in magento 2.4.7
  * _Fix note_: The system now correctly displays constructor parameters when executing the `dev:di:info` command, preventing any errors from occurring. Previously, executing this command resulted in an error due to a type mismatch in the argument.
  * _GitHub issue_: <https://github.com/magento/magento2/issues/38740>
  * _GitHub code contribution_: <https://github.com/magento/magento2/commit/0c53bbf7>
