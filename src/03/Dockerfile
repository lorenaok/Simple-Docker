FROM nginx:latest

RUN apt-get update && \
    apt-get install -y gcc libfcgi-dev spawn-fcgi

COPY server.c server.c
COPY nginx.conf etc/nginx/nginx.conf

# gcc server.c -o server -lfcgi
#   spawn-fcgi -p 8080 ./server

