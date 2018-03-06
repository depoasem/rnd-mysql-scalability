# Migrasi MySQL Master Slave ke MariaDB Galera Multimaster

MySQL server yang jalan saat ini, hampir semua table engine menggunakan
MyISAM. Berikut persiapan sebelum migrasi ke MariaDB Galera Multimaster :

1.  Full Backup database
2.  Setup mesin baru untuk MariaDB Galera Multimaster, minimum 3 nodes
3.  Convert Database MyISAM to InnoDB
4.  Migrasi Database schema include data to Mesin Baru (MySQL Galera Cluster)

ToDo :
- Untuk meminimalisir kerusakan / lost data, snapshot VM dan full backup database schema
- Paralel siapkan mesin baru MariaDB 10.0 dengan Multimaster Galera Cluster
- 
