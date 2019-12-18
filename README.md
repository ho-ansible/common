# Ansible role: common
Miscellaneous setup for Linux servers

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `default_domain`: to set FQDN of host
+ `timezone`: as string
+ `locales` (default: ["en_US.UTF-8", "UTF-8"]):
  list of [<locale>, <charset>] pairs.
  Chosen locales must exist in /usr/share/i18n/locales.
  First entry is set as system default.

## Dependencies
None

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
