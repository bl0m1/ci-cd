FROM python:3.11.3-alpine3.17

RUN apk add --no-cache git=2.38.5-r0 libffi-dev=3.4.4-r0 build-base=0.5-r3 libressl-dev=3.6.2-r0 zlib-dev=1.2.13-r0 && \
  pip3 install --no-cache-dir ansible-lint==6.15.0 ansible==7.5.0 yamllint==1.31.0 rich==12.3.5 Jinja2==3.1.2 MarkupSafe==2.1.2

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
