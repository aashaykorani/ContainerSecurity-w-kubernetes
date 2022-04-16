FROM mysql:latest

# ADD ./products.csv /products.csv
# ADD ./users.csv /users.csv
# ADD ./setup.sql /docker-entrypoint-initdb.d/setup.sql

COPY ./products.csv /products.csv
COPY ./users.csv /users.csv
COPY ./setup.sql /docker-entrypoint-initdb.d/setup.sql

# ENV MYSQL_ROOT_PASSWORD "thisisatestthing."


ENTRYPOINT ["/entrypoint.sh"]
CMD ["mysqld", "--secure-file-priv=/"]
#CMD ["--secure-file-priv=/"]
