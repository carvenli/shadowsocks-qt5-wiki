# Windows

Require Windows Vista or higher

1. Download latest prebuilt binaries from [releases](https://github.com/librehat/shadowsocks-qt5/releases).
2. Unpack it.
3. Execute `ss-qt5.exe`

# Linux

## Fedora/Red Hat Enterprise Linux

The Copr builds RPMs for Fedora 20, 21, 22 and RHEL 7. If you're using other RHEL-based distributions such as CentOS and Scientific Linux, you can just use the EPEL repo in Copr.

You can enable the repo via `dnf`:

```bash
sudo dnf copr enable librehat/shadowsocks
sudo dnf update
sudo dnf install shadowsocks-qt5
```

You may need to install dnf plugins by below command before you can enable copr repo.

```bash
sudo dnf install dnf-plugins-core
```

If your distribution doesn't have `dnf`, you can download the corresponding yum repo from [Copr](https://copr.fedoraproject.org/coprs/librehat/shadowsocks/) and put it under `/etc/yum.repos.d/`, then install `shadowsocks-qt5` via `yum`:

```bash
sudo yum update
sudo yum install shadowsocks-qt5
```

## Ubuntu

PPA is for Ubuntu >= 14.04.

```
sudo add-apt-repository ppa:hzwhuang/ss-qt5
sudo apt-get update
sudo apt-get install shadowsocks-qt5
```

## Debian

Make sure you've installed all dependencies for building `ss-qt5` by `sudo apt-get install qt5-qmake qtbase5-dev libqrencode-dev libqtshadowsocks-dev libappindicator-dev libzbar-dev libbotan1.10-dev`

Now run the command below, you'll get a deb package in upper directory.

```bash
dpkg-buildpackage -uc -us -b
```

Then, install it by `sudo dpkg -i shadowsocks-qt5-<VER_ARCH_ETC>.deb`.

## Arch

[AUR](https://aur.archlinux.org/packages/shadowsocks-qt5/) maintained by ykelvis

## Gentoo

[gentoo-zh](https://github.com/microcai/gentoo-zh) maintained by microcai

## Other distributions

Please follow instructions on [compiling](https://github.com/librehat/shadowsocks-qt5/wiki/Compiling) page to build it from source.

If you're maintaining other distributions' repository for `ss-qt5`, please open an issue to ask for adding it to this wiki page.