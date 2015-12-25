FROM ubuntu:14.04.3

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y make gcc wget
RUN wget http://downloads.sourceforge.net/project/idle3-tools/idle3-tools-0.9.1.tgz
RUN tar xzvf idle3-tools-0.9.1.tgz
WORKDIR /idle3-tools-0.9.1
RUN make
CMD ["/idle3-tools-0.9.1/idle3ctl", "-v"]
