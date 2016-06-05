# Postgres docker image with postgis based on alpine linux

Minimal alpine based docker postgres docker image with postgis extension.

## Usage

### Quick start

`docker run -d -p 5432:5432 hegand/postgres-postgis`

### Add master password:

`docker run -d -p 5432:5432 -e POSTGRES_PASSWORD=secretpass hegand/postgres-postgis`

### Attach a volume:

`docker run -d -p 5432:5432 -e POSTGRES_PASSWORD=secretpass -v /local/dir:/var/lib/postgresql/data hegand/postgres-postgis`

More info about the configs: [offical postgres image](https://hub.docker.com/_/postgres/)