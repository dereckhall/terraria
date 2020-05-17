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
* vanilla-1.4.0.2, vanilla-latest [(containers/vanilla/1.4.0.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.4.0.2/Dockerfile)
* vanilla-1.4.0.1, vanilla-latest [(containers/vanilla/1.4.0.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.4.0.1/Dockerfile)
* vanilla-1.3.5.3, vanilla-latest [(containers/vanilla/1.3.5.3/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.5.3/Dockerfile)
* vanilla-1.3.4.4 [(containers/vanilla/1.3.4.4/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.4.4/Dockerfile)
* vanilla-1.3.3.3 [(containers/vanilla/1.3.3.3/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.3.3/Dockerfile)
* vanilla-1.3.2.1 [(containers/vanilla/1.3.2.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.2.1/Dockerfile)
* vanilla-1.3.1.1 [(containers/vanilla/1.3.1.1/Dockerfile)](https://github.com/dereckhall/terraria/blob/master/containers/vanilla/1.3.1.1/Dockerfile)

### Quick reference
- Where to get help:
the [Terraria Forum](https://forums.terraria.org/index.php?forums/)

- Where to file issues:
https://github.com/dereckhall/terraria/issues

- Thanks to:
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

### dereckhall/terraria:vanilla-latest
Vanilla Terraria server is the server software provided by the developers of Terraria. This version has only basic features but it is updated along with the main game so it should always be up to date.

### FAQ
- I started the container but it keeps asking me to select a world, help?!
You need to ether start the server with an existing world, in which case the server will start automaticly. Or you need to run the continer interactivly using the -it flag. This will allow you to create a new world.

#### *Notes*
* More information about running a server is available in the [wiki](https://terraria.gamepedia.com/Server).

#### License

The MIT License (MIT)
Copyright (c) 2020 Brandon Skrtich
