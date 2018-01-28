FROM ubuntu:16.04

ADD ./scripts /scripts
ADD ./manifestfiles /manifestfiles

RUN chmod +x /scripts/* && \
    /scripts/install-dependencies && \
    useradd -m steam

USER steam
WORKDIR /home/steam

RUN /scripts/install-steamcmd && \
    /scripts/install-cstrike

COPY ./config/server.cfg /home/steam/games/cstrike/cstrike/server.cfg
COPY ./config/mapcycle.txt /home/steam/games/cstrike/cstrike/mapcycle.txt

CMD /scripts/start-server
