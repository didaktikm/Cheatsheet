PostgreSQL
===

.. autosummary::
   :toctree: generated

   SELECT * FROM pg_stat_activity WHERE pg_stat_activity.datname='mydb';
   SELECT pg_terminate_backend(pid) FROM pg_stat_activity WHERE datname = 'mydb';
