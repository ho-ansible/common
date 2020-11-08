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

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run before removing config from inventory.

## Dependencies
None.

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
