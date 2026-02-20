FROM postgres:16-alpine

RUN apk add --no-cache postgresql-contrib

COPY init.sql /docker-entrypoint-initdb.d/
