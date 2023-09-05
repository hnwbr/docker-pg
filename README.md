https://github.com/docker-library/docs/blob/master/postgres/README.md
https://github.com/felipewom/docker-compose-postgres
https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html

sudo docker run -i --rm postgres:15-alpine cat /usr/local/share/postgresql/postgresql.conf.sample > my-postgres.conf

sudo docker network create pg && \
sudo docker volume create var-lib-postgresql-data && \
sudo docker volume create var-lib-pgadmin

sudo mkdir bind
sudo mkdir bind/var-lib-pgadmin
sudo chown -R 5050:5050 ./bind/var-lib-pgadmin
