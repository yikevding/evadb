SQLite
==========

The connection to SQLite is based on the `sqlite3 <https://docs.python.org/3/library/sqlite3.html>`_ library.

Dependency
----------

* sqlite3


Parameters
----------

Required:

* `database` is the path to the database file to be opened. You can pass ":memory:" to create an SQLite database existing only in memory, and open a connection to it.

.. warning:: 

     If the ``database`` parameter is specified, EvaDB connects to the already existing ``sqlite`` database specified. Otherwise, it automatically creates a new ``sqlite`` database named ``evadb.db``.

Create Connection
-----------------

.. code-block:: text

   CREATE DATABASE sqlite_data WITH ENGINE = 'sqlite', PARAMETERS = {
        "database": "evadb.db"
   };
