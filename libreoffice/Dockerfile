FROM debian:jessie

RUN apt-get update
RUN apt-get install -y libreoffice
RUN apt-get clean

RUN mkdir /bootstrap
ADD start-libreoffice.sh /bootstrap/start.sh
RUN chmod u+x /bootstrap/start.sh

EXPOSE 8100
ENTRYPOINT ["/bootstrap/start.sh"]
