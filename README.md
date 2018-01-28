# Steam Dedicated Servers (with Docker)

Just some Steam game servers using Docker ;)

## Counter-Strike 1.6

Just run the command below to start the server:

``` bash
$ docker-compose up cstrike
```

> **Warning:** The first time you run this may take a while to set up everything because Steam [has a bug when downloading CS 1.6](https://developer.valvesoftware.com/wiki/SteamCMD#Only_the_HLDS_engine_is_downloaded).

All of the server configuration files can be found inside `cstrike/config` folder, have fun!
