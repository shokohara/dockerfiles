FROM ubuntu:14.04

RUN apt-get update
RUN apt-get install -y libssl1.0.0 curl wget

RUN curl -L -o utserver.tar.gz http://download-new.utorrent.com/endpoint/utserver/os/linux-x64-ubuntu-13-04/track/beta/
RUN curl -L -o webui.zip https://sites.google.com/site/ultimasites/files/utorrent-webui.2013052820184444.zip
#RUN wget https://github.com/psychowood/ng-torrent-ui/releases/download/v0.4.5/webui.zip

ADD utserver.tar.gz /opt
RUN cd /opt/ && ln -s /opt/$(ls /opt/|tail -1) /opt/utorrent-server

EXPOSE 6881
EXPOSE 8080

VOLUME ["/data"]

ENTRYPOINT ["/opt/utorrent-server/utserver"]
CMD ["-settingspath", "/opt/utorrent-server/"]
