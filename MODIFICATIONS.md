# Modifications

This repository contains a modified build of Arize Phoenix. The exact source
revision for each container image is identified by the image tag and OCI image
labels.

The changes add support for using a MySQL-compatible database as a Phoenix
storage backend. The implementation is intended to work through Phoenix's
existing `PHOENIX_SQL_DATABASE_URL` configuration surface, for example:

```text
PHOENIX_SQL_DATABASE_URL=mysql://user:password@host:3306/phoenix
```

The modified build has been tested with MySQL-compatible storage backends,
including MySQL and SeekDB in MySQL mode.

This build is not an official Arize AI release. Phoenix remains licensed under
the Elastic License 2.0; see `LICENSE` and `IP_NOTICE` for the upstream license
terms and notices.
