==========
PostgreSQL
==========


Просмотр соединений с базой
===========================
Для вывода соединений с определенной базой выполните::

   SELECT * FROM pg_stat_activity WHERE pg_stat_activity.datname='mydb';

DROPнуть активные коннекты
==========================
Разорвать активные сессии можно следуюжей командой::
   
   SELECT pg_terminate_backend(pid) FROM pg_stat_activity WHERE datname = 'mydb';
