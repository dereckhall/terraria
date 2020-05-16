# terraria

Docker images to run a Terraria Server. Images with [TShock Server](https://github.com/Pryaxis/TShock) or [Vanilla Server](https://terraria.gamepedia.com/Server) are available.


![Docker Image Size (tag)](https://img.shields.io/docker/image-size/beardedio/terraria/latest) ![MicroBadger Layers (tag)](https://img.shields.io/microbadger/layers/beardedio/terraria/latest) [![Docker Pulls](https://img.shields.io/docker/pulls/beardedio/terraria.svg)]() [![Docker Stars](https://img.shields.io/docker/stars/beardedio/terraria.svg)]()

### Usage
```
docker create -it \
  --name=terraria \
  -v <path to data>:/config \
  -e world=<world_file_name> \
  -p 7777:7777 \
  dereckh/terraria
```

Docker Images are avaiable on [Docker Hub](https://hub.docker.com/repository/docker/dereckh/terraria)

### Supported tags and respective `Dockerfile` links
* vanilla-1.4.0.1, vanilla-latest [(containers/vanilla/1.4.0.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.4.0.1/Dockerfile)
* vanilla-1.3.5.3, vanilla-latest [(containers/vanilla/1.3.5.3/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.5.3/Dockerfile)
* vanilla-1.3.4.4 [(containers/vanilla/1.3.4.4/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.4.4/Dockerfile)
* vanilla-1.3.3.3 [(containers/vanilla/1.3.3.3/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.3.3/Dockerfile)
* vanilla-1.3.2.1 [(containers/vanilla/1.3.2.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.2.1/Dockerfile)
* vanilla-1.3.1.1 [(containers/vanilla/1.3.1.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.1.1/Dockerfile)
* tshock-4.3.26, tshock-latest, latest [(containers/tshock/4.3.26/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.26/Dockerfile)
* tshock-4.3.25 [(containers/tshock/4.3.25/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.25/Dockerfile)
* tshock-4.3.24 [(containers/tshock/4.3.24/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.24/Dockerfile)
* tshock-4.3.23 [(containers/tshock/4.3.23/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.23/Dockerfile)
* tshock-4.3.22 [(containers/tshock/4.3.22/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.22/Dockerfile)
* tshock-4.3.20 [(containers/tshock/4.3.20/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.20/Dockerfile)
* tshock-4.3.19 [(containers/tshock/4.3.19/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.19/Dockerfile)
* tshock-4.3.18 [(containers/tshock/4.3.18/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.18/Dockerfile)
* tshock-4.3.17 [(containers/tshock/4.3.17/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.17/Dockerfile)
* tshock-4.3.16 [(containers/tshock/4.3.16/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock/4.3.16/Dockerfile)
* tshock-dev-949, tshock-dev-latest [(containers/tshock-dev/949/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/949/Dockerfile)
* tshock-dev-934 [(containers/tshock-dev/934/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/934/Dockerfile)
* tshock-dev-932 [(containers/tshock-dev/932/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/932/Dockerfile)
* tshock-dev-930 [(containers/tshock-dev/930/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/930/Dockerfile)
* tshock-dev-928 [(containers/tshock-dev/928/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/928/Dockerfile)
* tshock-dev-926 [(containers/tshock-dev/926/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/926/Dockerfile)
* tshock-dev-924 [(containers/tshock-dev/924/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/924/Dockerfile)
* tshock-dev-917 [(containers/tshock-dev/917/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/917/Dockerfile)
* tshock-dev-915 [(containers/tshock-dev/915/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/915/Dockerfile)
* tshock-dev-913 [(containers/tshock-dev/913/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/tshock-dev/913/Dockerfile)

### Quick reference
- Where to get help:
the [TShock Forums](https://github.com/Pryaxis/TShock/discussions) or the [Terraria Forum](https://forums.terraria.org/index.php?forums/)

- Where to file issues:
https://github.com/dereckhall/terraria/issues

- Maintained by:
[Brandon Skrtich of Bearded.io](https://www.bearded.io/#footer)

- Supported Docker versions:
[the latest release](https://github.com/docker/docker-ce/releases/latest) (down to 1.8 on a best-effort basis)

### What is Terraria Server?
A Terraria server provides a platform for players to connect over the internet or other network for multiplayer games of [Terraria](https://terraria.org/).

## How to use

### Generating a new world
To run with out user intervention Terraria Server needs to be configure to use an already generated world. This means you can use one that you have already generated or you can generate one via docker by running this command:
```
sudo docker run -it -p 7777:7777 \
    -v $HOME/terraria/config:/config \
    --name=terraria \
    dereckh/terraria
```
You can then follow the prompts to create a new world.

### Starting your server with a preexisting world
The world file needs to exist in the config folder.
To start a server using an already generated world, use this command:
```
sudo docker run -dit \
  --name=terraria \
  -v $HOME/terraria/config:/config \
  -e world=<world_file_name> \
  -p 7777:7777 \
  dereckh/terraria
```

If you get an error from docker saying the container name already exists, it means you need to remove your old docker container process.
`sudo docker rm terraria`

If you want to reattach to any running containers:
`sudo docker attach terraria`
Now you can execute any commands to the terraria server. Ctrl-p Ctrl-q will detatch you from the process.

### dereckhall/terraria:tshock-latest
TShock is a server modification for Terraria, written in C#, and based upon the Terraria Server API. It uses JSON for configuration management, and offers several features not present in the Terraria Server normally.

### dereckhall/terraria:tshock-dev-latest
TShock dev are unreleased development builds of TShock. These builds may be unstable but they are updated faster then the released versions so they support new versions of Terraria faster.

### dereckhall/terraria:vanilla-latest
Vanilla Terraria server is the server software provided by the developers of Terraria. This version has only basic features but it is updated along with the main game so it should always be up to date.

If a docker image isn't available of the latest versions please [contact us](https://www.bearded.io/#footer) about the new release so we can update this repo.

### FAQ
- Can I manage my own plugins for tshock?
Yes, if you want manage you own plugins for tshock containers, you can add a volume mount to your docker command via `-v <path to plugins folder>:/tshock/ServerPlugins`. If you want to maintain any of the plugins that ship with tshock, you will need to copy them into the ServerPlugins folder. Mounting the plugins folder will override the plugins that ship with tshock.
- I started the container but it keeps asking me to select a world, help?!
You need to ether start the server with an existing world, in which case the server will start automaticly. Or you need to run the continer interactivly using the -it flag. This will allow you to create a new world.

#### *Notes*
* Please check the [TShock instructions](https://tshock.readme.io/docs/getting-started) for properly installing and configuring your terraria server.
* Any [additional command-line instructions](https://tshock.readme.io/docs/command-line-parameters) can be added to the end of either method for launching a server.  Docker maps the $HOME/terraria/world linux-host folder to the /tshock/world container-folder.
* More information about running a server is available in the [wiki](https://terraria.gamepedia.com/Server).

#### License

The MIT License (MIT)
Copyright (c) 2020 Brandon Skrtich
