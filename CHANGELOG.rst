0.4.1 2022-10-09
----------------

* Bugfix add missing aiosqlite dependency

0.4.0 2022-10-08
----------------

* Support SQLite databases.
* Bugfix ensure that exceptions are not propagated, unless
  specifically set. This prevents connection exhaustion on errors.

0.3.0 2022-08-23
----------------

* Require the connection lock earlier in iterate.
* Acquire the connection lock on Transaction.
* Add a db-schema command to output the entity relation diagram.

0.2.0 2022-04-12
----------------

* Add a lock on connection operations to ensure only one concurrent
  operation per connection (use multiple connections).
* Add a default per request connection on g, so that g.connection can
  be used in request contexts.
* Switch to github rather than gitlab.

0.1.0 2022-03-07
----------------

* Basic initial release.
