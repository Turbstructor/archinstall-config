# NOTE: This repository is NOT OFFICIAL and I'm NOT AFFILIATED with the official `archinstall` repository.

# `archinstall-config`

Personal `archinstall` configuration for installing archlinux in multiple environments: 'laptop' and 'workspace' at the time I wrote this `README.md` file.

Used with `archinstall`'s *guided* installation script. See [Guided Installation#`--config`](https://archinstall.archlinux.page/installing/guided.html#config) for detailed explanation of how to use customized configuration files.

## Usage

1. Boot with Archlinux ISO
2. Download `*.json` files from this repository using `curl` (if you want to pass the file link(like `https://github.com/Turbstructor/archinstall-config/blob/main/turbArch.json`) you can skip this step)
3. Run `archinstall` with flags `--config`, `--creds`, and `--disk_layouts`.
4. Confirm loaded configurations and proceed to installation.