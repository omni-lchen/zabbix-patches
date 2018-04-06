# zabbix-patches

* htmlentitiy-decode: add htmlentitydecode function in Post fields of a HTTP test, such as {{macro}.htmlentitydecode()}, see urlencode in zabbix web monitoring, tested in zabbix 3.4.x



Notes: You need to recompile the zabbix source and replace current zabbix proxy or zabbix server bin file with compiled version.

Example command lines to recompile zabbix server or proxy using mysql database
* ./configure --prefix=/tmp/zabbix --enable-server --with-mysql --with-net-snmp --with-ssh2 --with-unixodbc --with-libcurl --with-libxml2 --with-openssl
* ./configure --prefix=/tmp/zabbix --enable-proxy --with-mysql --with-net-snmp --with-ssh2 --with-unixodbc --with-libcurl --with-libxml2 --with-openssl

Example command lines to recompile zabbix server or proxy using postgres database
* ./configure --prefix=/tmp/zabbix --enable-server --with-postgresql --with-net-snmp --with-ssh2 --with-unixodbc --with-libcurl --with-libxml2 --with-openssl
* ./configure --prefix=/tmp/zabbix --enable-proxy --with-postgresql --with-net-snmp --with-ssh2 --with-unixodbc --with-libcurl --with-libxml2 --with-openssl