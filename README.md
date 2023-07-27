https://github.com/docker-library/docs/blob/master/postgres/README.md
https://github.com/felipewom/docker-compose-postgres
https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html

sudo docker run -i --rm postgres:15-alpine cat /usr/local/share/postgresql/postgresql.conf.sample > my-postgres.conf

sudo docker volume create vol_pg15_data && \
sudo docker network create net_pg
