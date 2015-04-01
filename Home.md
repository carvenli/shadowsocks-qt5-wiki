# 中文文档

原**用户指南**被拆成了两部分，分别是

- [安装指南](https://github.com/librehat/shadowsocks-qt5/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
- [使用手册](https://github.com/librehat/shadowsocks-qt5/wiki/%E4%BD%BF%E7%94%A8%E6%89%8B%E5%86%8C)

如Wiki需更改，请提交issue！

# English Documentation

How to
- [Compile](https://github.com/librehat/shadowsocks-qt5/wiki/Compiling)
- [Install](https://github.com/librehat/shadowsocks-qt5/wiki/Installation)

File an issue if there is any modifications needed.

# Libraries used in releases

## Botan
You can download pre-compiled `botan` libraries linked in Windows builds [here] (http://file.librehat.com/botan/). Note: they're statically linked. The filename indicates build information.

## Qt
For Windows builds, self-compiled statically linked Qt libraries are used. Because they're directly compiled from Qt source without any source modifications, you can compile it yourself using Qt's source code.

## libQtShadowsocks
See my [libQtShadowsocks](https://github.com/librehat/libQtShadowsocks) project.

## zbar
Pre-compiled statically linked libraries are provided in `3rdparty` directory. You can get my modified source code [here](http://file.librehat.com/).

## qrencode
Pre-compiled statically linked libraries are provided in `3rdparty` directory. There is no source code modification. You can download the source code from their website and compile it yourself.