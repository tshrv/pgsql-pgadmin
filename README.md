# PostgreSQL and PGAdmin

## Requirments
`.env` file with following parameters -
1. PGSQLDB_CONTAINER_NAME
2. PGSQLDB_POSTGRES_USER
3. PGSQLDB_POSTGRES_PASSWORD
4. PGSQLDB_POSTGRES_DB [optional]
5. PGSQLDB_DATA_DIR
6. PGADMIN_CONTAINER_NAME
7. PGADMIN_PORT
8. PGADMIN_DEFAULT_EMAIL
9. PGADMIN_DEFAULT_PASSWORD

## Run
```bash
docker-compose up --build -d
```

## PGAdmin
Accessible on `http://127.0.0.1:<PGADMIN_PORT>`

## PSQL
Accessible via -
```bash
docker exec -it <PGSQLDB_CONTAINER_NAME> psql -U <PGSQLDB_POSTGRES_USER>
```