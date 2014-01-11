graphite-rethinkdb
==================
A plugin for using graphite-web with the cassandra-based Cyanite storage
backend.

**Requires at least Graphite-web 0.10.X, which is currently unreleased. You'll
need to install it from source.**

Installation
------------

::

    pip install graphite-rethinkdb

Usage
-----

In your graphite's ``local_settings.py``::

    STORAGE_FINDERS = (
        'rethinkdb.RethinkdbFinder',
    )

    RETHINKDB_URL = 'http://host:port'

Where ``host:port`` is the location of the RethinkDB HTTP API.
