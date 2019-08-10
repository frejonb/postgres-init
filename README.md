# postgres-init docker image
Postgres 9.6 docker image with support for initialization SQL command

# Usage
Sames as https://hub.docker.com/_/postgres but adds an additional environment variable `POSTGRES_CMDS`:

```
docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword \
-e POSTGRES_CMDS='CREATE DATABASE \"mydb\"; \n CREATE DATABASE \"mydb2\";' \
-d postgres
```