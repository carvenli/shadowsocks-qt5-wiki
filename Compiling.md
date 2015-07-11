## Dependencies

Make sure you've installed all dependent **development** packages (with `-dev` or `-devel`).

- `qt5-qtbase` >= 5.2 (`qtbase5` in Debian/Ubuntu)
- `qrencode` (`libqrencode` in Debian/Ubuntu)
- `libQtShadowsocks` >= 1.6.1 (`libqtshadowsocks` in Debian/Ubuntu. **DON'T** use the trunk code)
- `botan` >= 1.10 (`libbotan1.10` in Debian/Ubuntu)
- `zbar` (`libzbar0` in Debian/Ubuntu)
- `libappindicator` (`libappindicator1` in Debian/Ubuntu)

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
|DEFINES+="mingw64"|Use pre-compiled libraries from `mingw64` instead of `mingw32` (only on Windows)|NULL|
