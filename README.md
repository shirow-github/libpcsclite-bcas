# libpcsclite-bcas

*Current Version:* 1.0.0

libpcscliteを改造し、B-CASカードの動作をソフトウェアでエミュレートします。

----
##  インストール方法
```bash
$ sudo apt -y install autoconf libtool
$ ./bootstrap  
$ ./configure  
$ make  
$ sudo make install  
$ sudo /sbin/ldconfig  
```

## アンインストール方法
```bash
$ sudo make uninstall  
$ sudo /sbin/ldconfig  
```
