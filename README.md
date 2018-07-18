### Starting Point for Rails App in Docker ###

* ensure docker is installed
* ensure docker-compose is installed

run `docker-compose run web rails new . --force --database=postgresql`

on linux systems:
run `sudo chown -R $USER:$USER .`


run `docker-compose build`

set host `db` in database config, and user / password

run `docker-compose up -d`

create db: `docker-compose run web rake db:create`

open `http://localhost:3000`
