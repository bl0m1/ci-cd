FROM python:3.11.0a7-alpine3.15

RUN apk add --no-cache git=2.34.2-r0 libffi-dev=3.4.2-r1 build-base=0.5-r2 libressl-dev=3.4.3-r0 zlib-dev=1.2.12-r1 && \
  pip3 install --no-cache-dir ansible-lint==6.0.2 ansible==5.7.1 yamllint==1.26.3 rich==12.3 Jinja2==3.1.2 MarkupSafe==2.1.1

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
