FROM weilan6222/baseimage:latest

MAINTAINER Wei Lan <wei.lan6222@gmail.com>

COPY run-certbot.sh /root/certbot/run-certbot.sh

RUN apt-get update
RUN apt-get install -y letsencrypt

ENTRYPOINT bash -c "bash /root/certbot/run-certbot.sh && sleep infinity"
