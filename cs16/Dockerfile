FROM ubuntu:16.04

RUN apt update -y && \
    apt upgrade -y && \
    apt install -y curl lib32gcc1 && \
    mkdir /var/steam && \
    cd /var/steam && \
    curl -sqL "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz" | tar zxvf - && \
    /var/steam/steamcmd.sh +quit

# RUN ["/var/steam/steamcmd.sh", "+login anonymous", "+force_install_dir ./cs16/", "+app_update 90 validate", "+quit"]
