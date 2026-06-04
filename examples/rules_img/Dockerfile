FROM debian:trixie-20260518-slim

ENV LC_ALL=C.UTF-8 \
    LANG=C.UTF-8 \
    LANGUAGE=C.UTF-8

RUN apt-get -y update \
    && apt-get -y install git \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENTRYPOINT [ "/usr/bin/git" ]
CMD [ "--version" ]
