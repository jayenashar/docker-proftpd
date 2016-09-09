# docker-proftpd

A 145.3 MB docker image for proftpd.

Can be extended with another Dockerfile like this:

```
FROM proftpd

VOLUME /home /var/log

COPY etc/proftpd/conf.d/ /etc/proftpd/conf.d/
# open ports for passive mode
EXPOSE 49152-49160
```
