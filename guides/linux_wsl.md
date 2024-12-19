# Prepare Your Build Environment For Linux/WSL
> [!TIP]
> **Note for WSL users**: By default, the installation process will clone the QMK repository into your WSL home directory, but if you have cloned manually, ensure that it is located inside the WSL instance instead of the Windows filesystem (ie. not in `/mnt`), as accessing it is currently [extremely slow](https://github.com/microsoft/WSL/issues/4197).
## Prerequisites
You will need to install Git and Python. It's very likely that you already have both, but if not, one of the following commands should install them:
* Debian / Ubuntu / Devuan: `sudo apt install -y git python3-pip`
* Fedora / Red Hat / CentOS: `sudo yum -y install git python3-pip`
* Arch / Manjaro: `sudo pacman --needed --noconfirm -S git python-pip libffi`
* Void: `sudo xbps-install -y git python3-pip`
* Solus: `sudo eopkg -y install git python3`
* Sabayon: `sudo equo install dev-vcs/git dev-python/pip`
* Gentoo: `sudo emerge dev-vcs/git dev-python/pip`
## Installation
Install the QMK CLI by running:
```sh
python3 -m pip install --user qmk
```
## Community Packages
These packages are maintained by community members, so may not be up to date or completely functional. If you encounter problems, please report them to their respective maintainers.
On Arch-based distros you can install the CLI from the official repositories (NOTE: at the time of writing this package marks some dependencies as optional that should not be):
```sh
sudo pacman -S qmk
```
You can also try the `qmk-git` package from AUR:
```sh
yay -S qmk-git
```
