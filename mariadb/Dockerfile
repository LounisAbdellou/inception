FROM debian:bullseye

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y mariadb-server netcat

COPY ./mariadb.sh /mariadb.sh

RUN chmod +x /mariadb.sh

ENTRYPOINT ["./mariadb.sh"]
