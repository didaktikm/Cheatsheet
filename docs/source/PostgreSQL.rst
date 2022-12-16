==========
PostgreSQL
==========


Просмотр соединений с базой::

   SELECT * FROM pg_stat_activity WHERE pg_stat_activity.datname='mydb';

DROPнуть активные коннекты::
   
   SELECT pg_terminate_backend(pid) FROM pg_stat_activity WHERE datname = 'mydb';
