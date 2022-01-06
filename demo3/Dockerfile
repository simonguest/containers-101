FROM ubuntu:latest
RUN apt update
RUN apt install -y vim python curl
RUN mkdir /var/www
COPY ./index.html /var/www/.
EXPOSE 8000
WORKDIR /var/www
CMD python -m SimpleHTTPServer
