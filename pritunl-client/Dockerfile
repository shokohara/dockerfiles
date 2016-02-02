FROM debian:jessie
RUN apt-get update
RUN apt-get upgrade -y
RUN echo 'deb http://repo.pritunl.com/stable/apt jessie main' >> /etc/apt/sources.list.d/pritunl.list
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv CF8E292A
RUN apt-get update
RUN apt-get install -y pritunl-client
ADD entrypoint.sh /
ENTRYPOINT ["./entrypoint.sh"]
