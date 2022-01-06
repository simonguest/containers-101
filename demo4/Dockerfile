FROM ubuntu:latest
RUN apt update
RUN apt install -y vim python curl
EXPOSE 8000
WORKDIR /var/www
CMD python -m SimpleHTTPServer
