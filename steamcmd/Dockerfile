FROM ubuntu:16.04

ADD ./scripts /scripts

RUN chmod +x /scripts/* && \
    /scripts/install-dependencies && \
    useradd -m steam

USER steam
WORKDIR /home/steam

RUN /scripts/install-steamcmd

ENTRYPOINT /home/steam/steamcmd.sh
