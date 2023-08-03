https://github.com/docker-library/docs/blob/master/postgres/README.md
https://github.com/felipewom/docker-compose-postgres
https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html

sudo docker run -i --rm postgres:15-alpine cat /usr/local/share/postgresql/postgresql.conf.sample > my-postgres.conf

sudo docker volume create vol_pg15_data && \
sudo docker network create net_pg

sudo docker-compose -f pg15alpine.yaml up

sudo chown -R 5050:5050 ./bind-var-lib-pgadmin

sudo docker-compose -f pgadmin4.yaml up
