# docker-db-postgres

To start the environment execute the following command:

```Shell
docker compose -f docker-compose.yml up --build
```

To run the containers run in the background:

```Shell
docker compose -f docker-compose.yml up --build -d
```

```shell
$ docker exec -it postgres-docker-db-1 psql -U postgres -W postgres
```
```shell
postgres=# \dt+
                                    List of relations
 Schema |   Name   | Type  |  Owner   | Persistence | Access method | Size  | Description 
--------+----------+-------+----------+-------------+---------------+-------+-------------
 public | budget   | table | postgres | permanent   | heap          | 16 kB | 
 public | category | table | postgres | permanent   | heap          | 16 kB | 
 public | entry    | table | postgres | permanent   | heap          | 16 kB | 
 public | user     | table | postgres | permanent   | heap          | 16 kB | 
(4 rows)
```
