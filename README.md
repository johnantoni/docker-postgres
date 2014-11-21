docker-postgres
===============

standard postgres docker script

#### start boot2docker (osx)

    boot2docker start
    
#### generate

    docker build -t local-postgres .
    
#### run

    docker run --rm -P --name local-pg local-postgres

#### container linking

    docker run --rm -t -i --link local-pg:pg local-postgres bash
    
* http://docs.docker.com/examples/postgresql_service/
