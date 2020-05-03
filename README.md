# libpcsclite-bcas

libpcscliteを改造し、B-CASカードの動作をソフトウェアでエミュレートします。

----
##  インストール方法

$ ./bootstrap  
$ ./configure  
$ make  
$ sudo make install  
$ sudo mv /usr/lib/libpcsclite.so.1.0.0{,.bak}  
$ sudo rm /usr/lib/libpcsclite.so /usr/lib/libpcsclite.so.1  
$ sudo ln -s /usr/local/lib/libpcsclitebcas.so.0.0.0 /usr/lib/libpcsclite.so    
$ sudo /sbin/ldconfig  

## アンインストール方法

$ sudo make uninstall  
$ sudo mv /usr/lib/libpcsclite.so.1.0.0.bak /usr/lib/libpcsclite.so.1.0.0  
$ sudo rm /usr/lib/libpcsclite.so /usr/lib/libpcsclite.so.1 /usr/lib/libpcsclitebcas.so.0  
$ sudo ln -s /usr/lib/libpcsclite.so.1.0.0 /usr/lib/libpcsclite.so  
$ sudo /sbin/ldconfig  
