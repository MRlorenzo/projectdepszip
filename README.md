# projectdepszip
备份项目串口依赖压缩文件

npm serialport模块是node原始模块，并且从npm下载的预编译版本和electron当前版本不兼容。
因此serialport模块需要重新编译，这里用到的编译工具模块为electron-rebuild.
但electron-rebuild依赖的node-gyp模块需要下载c++编译环境, 安装windows-build-tools 可以解决这个问题。
但serialport是用python2.7写的，因此还需要有python2.7的环境，最可怕的就是目前最新的python3.x居然和python2.7不兼容。
因此，为了避免麻烦索性把serialport预编译当前用到的版本并且备份。
