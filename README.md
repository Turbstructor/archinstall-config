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

## Usage (with configuration files)
1. Boot with Archlinux ISO Image.
2. Prepare configuration files. You could use them from previous steps, but since I uploaded them here, I'd download them via `curl`(FYI: Archlinux ISO image does *not* contain `wget` or `git`), e.g.:
    ```bash
    curl -O https://raw.githubusercontent.com/Turbstructor/archinstall-config/main/workstation/user_configuration.json
    curl -O https://raw.githubusercontent.com/Turbstructor/archinstall-config/main/workstation/user_credentials.json
    ```
    Modify the downloaded files to your preferences.
3. Run `archinstall` with `--config` and `--creds` options (with each configiration file as argument, such as `user_configuration.json` and `user_credentials.json`).
    ```bash
    archinstall --config user_configuration.json --creds user_credentials.json
    ```
    You can pass **remote URL** instead of file path:
    ```bash
    archinstall --config <your_link_to_configuration_file> --creds <your_link_to_credentials_file>
    ```
4. Confirm loaded configurations and proceed to installation if all seems to be ready.