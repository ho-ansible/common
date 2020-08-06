# Ansible role: common
Miscellaneous setup for Linux servers:

+ Install and configure less, vim, and htop
+ Set hostname, timezone, and locale
+ Configure apt auto-upgrade

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `default_domain`: to set FQDN of host
+ `timezone`: as string
+ `locale` (default: `en_US.UTF-8`): system default `LANG`

## Dependencies
None

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
