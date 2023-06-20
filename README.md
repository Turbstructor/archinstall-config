# `archinstall-config`

Personal `archinstall` configuration for installing archlinux in two desktops(`desktop` and `workspace`) and a laptop.<br>
Used with `archinstall`'s guided installation script.

## Usage

0. Boot with Archlinux ISO
1. Download `*.json` files from this repository using `curl`
2. Run `archinstall` with flags `--config`, `--creds`, and `--disk_layouts`. See more at [Archinstall Documentation: Guided Installation](https://archinstall.readthedocs.io/installing/guided.html)
3. Confirm pre-loaded configurations and proceed to installation.

## TODO
- Add configuration files for `desktop`
- Find alternative/fixing way for 'exception during installing "server" profile' in `workspace`.