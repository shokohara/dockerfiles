FROM ubuntu:15.10

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y wget
RUN wget http://repo.zabbix.com/zabbix/2.4/ubuntu/pool/main/z/zabbix-release/zabbix-release_2.4-1+trusty_all.deb
RUN dpkg -i zabbix-release_2.4-1+trusty_all.deb
