# NOTE: This repository is NEITHER OFFICIAL NOR AFFILIATED with the official `archinstall` repository.

# `archinstall-config`

Personal `archinstall` configuration for installing archlinux in multiple environments: 'laptop' and 'workstation' at the time I wrote this `README.md` file.

Used with `archinstall`'s *guided* installation script. See [Guided Installation](https://archinstall.archlinux.page/installing/guided.html#guided-installation) for detailed explanation of how to make and use configuration files.

## How to make configuration files

1. In Archlinux, install the `archinstall` package:
    ```bash
    sudo pacman -S archinstall
    ```
2. Run `archinstall` *with root privileges* and *with `--dry-run` option*(in safe mode).
    ```bash
    sudo archinstall --dry-run
    ```
3. Set installation options to your preferences.
4. `Save configuration` to your location.

## Usage

1. Boot with Archlinux ISO
2. Run `archinstall` with `--config` and `--creds` options (with each configiration file as argument. ex) `user_configuration.json` and `user_credentials.json`).
    ```bash
    archinstall --config user_configuration.json --creds user_credentials.json
    ```
    Or if you want to get the files from remote locations(like me here):
    ```bash
    archinstall --config <your_link_to_configuration_file> --creds <your_link_to_credentials_file>
    ```
3. Confirm loaded configurations and proceed to installation.