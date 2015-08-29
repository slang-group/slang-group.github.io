---
layout: api
title:  PostgreSQL
date:   2015-08-29 15:49:10
categories: databases
---

PostgreSQL supports [several different text encodings](http://www.postgresql.org/docs/9.4/static/multibyte.html).

To support Unicode characters including Emoji in the current version of PostgreSQL, select the UTF8 encoding when you create the database:

```
initdb -E UTF8
```

In SQL you can run

```
CREATE DATABASE sample_name WITH ENCODING 'UTF8';
```

## Older versions

On [PostgreSQL 8.0 and earlier](http://www.postgresql.org/docs/8.0/static/multibyte.html), you should use 'UNICODE' instead of 'UTF8'.

Multibyte UNICODE encoding was made available for the first time in PostgreSQL 7.1 and 7.2, but you need to compile PostgreSQL with [--enable-multibyte=UNICODE](http://www.postgresql.org/docs/7.1/static/multibyte.html). Starting in 7.3, it was built-in.
