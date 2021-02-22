![Java CI with Maven](https://github.com/Brest-Java-Course-2021/afedasiuk/workflows/Java%20CI%20with%20Maven/badge.svg)

# Brest Java Course 2021 (winter)


## Using Docker to simplify development (optional)

You can use Docker.
A number of docker-compose configuration are available in the [./docker](./docker) folder to launch required third party services.


### Postgresql

For example, to start a postgresql database in a docker container, run:

```
docker-compose -f docker/postgresql.yml up -d
```

To stop it and remove the container, run:

```
docker-compose -f docker/postgresql.yml down
```

### Oracle XE


Create Oracle XE image first, see:
[deliver-oracle-database-18c-express-edition-in-containers](https://blogs.oracle.com/oraclemagazine/deliver-oracle-database-18c-express-edition-in-containers)

For example, to start a Oracle XE database in a docker container, run:

sudo chown 54321:54321 ~/oracle/volumes/xedb/oradata


```
docker-compose -f docker/oraclexe.yml up -d
```

To stop it and remove the container, run:

```
docker-compose -f docker/oraclexe.yml down
```
