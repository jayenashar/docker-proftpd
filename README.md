# docker-proftpd

A 145.3 MB docker image for proftpd.  If you want something smaller, look at alpine linux: https://github.com/pockost/docker-proftpd

Can be extended with another Dockerfile like this:

```
FROM proftpd

VOLUME /home /var/log

COPY etc/proftpd/conf.d/ /etc/proftpd/conf.d/
# open ports for passive mode
EXPOSE 49152-49160
```
