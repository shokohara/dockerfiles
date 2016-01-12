FROM ubuntu:15.10

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y git libcurl4-nss-dev libjansson-dev libssl-dev build-essential automake
RUN git clone https://github.com/tpruvot/cpuminer-multi.git
RUN cd cpuminer-multi && ./build.sh
