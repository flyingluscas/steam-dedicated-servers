FROM ubuntu:16.04

ADD ./scripts /scripts

RUN chmod +x /scripts/* && \
    /scripts/install-dependencies && \
    /scripts/install-steamcmd && \
    /scripts/install-cstrike

EXPOSE 27015
EXPOSE 27015/UDP
EXPOSE 27020/UDP
EXPOSE 26900/UDP
