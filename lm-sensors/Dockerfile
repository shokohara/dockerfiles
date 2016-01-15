FROM ubuntu:15.10

RUN apt-get update
RUN apt-get install -y lm-sensors hddtemp
RUN sensors-detect
RUN service kmod start
