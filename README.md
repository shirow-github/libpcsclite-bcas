# libpcsclite-bcas

libpcscliteを改造し、B-CASカードの動作をソフトウェアでエミュレートします。

----
##  インストール方法

$ make  
$ sudo cp -a libpcsclite.so.1.0.0 /usr/lib    ※x64の場合は、/usr/lib64  
$ sudo /sbin/ldconfig  
