# Postgres database Application

Postgres application with a volume to persistent the data. 

__NOTE: The volume remains alive as long as the application is deployed. When the app is deleted, the volume will be deleted too.__

## Application params

* __database__:  database name. This param is required.
* __user__ : database user. This param is required.
* __password__: user password. This param is required.
* __volume_name__: the volume name. This param is NOT required.
* __volume__: volume size. This param is NOT required.

## References

* [Postgres](https://www.postgresql.org/)

Database credentials: admin/admin
Database: postgresdb
