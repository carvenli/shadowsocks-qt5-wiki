## Dependencies

Make sure you've installed all dependent **development** packages (with `-dev` or `-devel`).

- `qt5-qtbase` >= 5.2 (`qtbase5` in Debian/Ubuntu)
- `qrencode` (`libqrencode` in Debian/Ubuntu)
- `libQtShadowsocks` >= 1.6.0 (`libqtshadowsocks` in Debian/Ubuntu)
- `botan` >= 1.10 (`libbotan1.10` in Debian/Ubuntu)
- `zbar` (`libzbar0` in Debian/Ubuntu)
- `libappindicator` (optional, `libappindicator1` in Debian/Ubuntu, only if you want to build with `appindicator` support)

## Compiling

```
qmake INSTALL_PREFIX=/usr
make
make install
```

Some useful special arguments for `qmake` command

|Arguments|Usage|Default Value|
|---------|------|-------|
|INSTALL_PREFIX="/usr"|Specify the installation prefix directory|/usr|
|BOTAN_VER="1.10"|Specify the `botan` library version|1.10|
|DEFINES+="UBUNTU_UNITY"|Turn on `appindicator` support|NULL|
|DEFINES+="mingw64"|Use pre-compiled libraries from `mingw64` instead of `mingw32` (only for Windows)|NULL|

Historically, application indicator was only used on Unity desktop environment. That's why the name `UBUNTU_UNITY` is picked for application indicator support. But it's no longer just a Ubuntu thing and should be considered distro-neutral. Therefore, for the sake of consistency, the name `UBUNTU_UNITY` remains unchanged.