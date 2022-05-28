# Postgres

### Build

    docker-compose up


## Extra
using custom port 5434

#### Copy dump to container
    sudo docker cp xx.backup postgres_container:/media
    sudo docker cp xx.dump postgres_container:/media


### Create Database
    psql -U postgres -h localhost -c 'CREATE DATABASE "dbase";'


#### Restore dump
    pg_restore -U postgres -d dbase < xx.backup