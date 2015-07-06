---
layout: api
title:  RethinkDB
date:   2015-07-05 16:22:10
categories: databases
---

To support all Unicode characters in RethinkDB, [use version 1.13 or higher](https://github.com/rethinkdb/rethinkdb/issues/2446).

Some RethinkDB drivers might not expect responses from the database to include 4-byte encoded
characters (newer additions to Unicode, including Emoji). Test these on a case-by-case basis.
