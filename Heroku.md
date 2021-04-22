# Heroku

PostgreSQL database restore locally from dump:

```
pg_restore --verbose --clean --no-acl --no-owner -h localhost -d <db_name> <Path to copy of Heroku DB dump>

```
