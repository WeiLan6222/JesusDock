FROM abiosoft/caddy:latest


MAINTAINER Wei Lan <wei.lan6222@gmail.com>

ARG plugins="cors git"

## ARG plugins="cors cgi cloudflare azure linode"


RUN caddyplug install ${plugins}
    

EXPOSE 80 443 2015

WORKDIR /var/www/public

CMD ["/usr/bin/caddy", "-conf", "/etc/Caddyfile"]
