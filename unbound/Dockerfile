FROM ubuntu:14.04

RUN apt-get -y update
RUN apt-get -y install aptitude
RUN aptitude -y install unbound

CMD ["-d", "-c", "/conf/unbound.conf"]

ENTRYPOINT ["unbound"]

EXPOSE 53/udp
