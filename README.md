# Ansible role: common
Miscellaneous setup for Linux servers:

+ Install and configure less, vim, and htop
+ Set hostname, timezone, and locale
+ Configure apt auto-upgrade
+ Upgrades kernel to backports (if desired)
+ Install initramfs-tools and provide handler to regenerate

## Requirements
Debian buster, bullseye

## Role Variables
+ `default_domain`: to set FQDN of host
+ `timezone`: as string
+ `locale` (default: `en_US.UTF-8`): system default `LANG`
+ `apt_repo` (default: Debian mirror autoselect): URL to package repository
+ `use_backports_kernel` (default: false): install kernel from backports repo
+ `config_files`: dictionary of (filename, contents) pairs, for
  arbitrary config files

## Handlers
+ `update initramfs`: regenerates the ram disk used by the kernel
  to find the root filesystem during boot

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run before removing config from inventory.

## Dependencies
None.

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
