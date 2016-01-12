FROM ubuntu:15.10

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y wget
RUN wget http://prdownloads.sourceforge.net/webadmin/webmin_1.770_all.deb
RUN apt-get install -y perl libnet-ssleay-perl openssl libauthen-pam-perl libpam-runtime libio-pty-perl python
RUN apt-get install -y apt-show-version
RUN dpkg --install webmin_1.770_all.deb
CMD ["/idle3-tools-0.9.1/idle3ctl", "-v"]
