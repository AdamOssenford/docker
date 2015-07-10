Docker 1.7.1 Fork for Raspberry Pi
==================================

![Docker L](docs/static_files/docker-logo-compressed.png "Docker")

This is a fork of the docker 1.7.1 rc3 build.  The Dockerfile has been modified to compile on a Raspberry Pi2.  Various Pi  package dependencies are required to successfully build.  Hopefully a list of those will make it to this readme in the future.

The operating system on the Raspberry Pi is from hypriot.  Please visit their site and download the flash utility to get your Pi up and running with docker 1.5.  [Hypriot Flash Tool](https://github.com/hypriot/flash) [HypriotOS used](http://downloads.hypriot.com/hypriot-rpi-20150329-140334.img.zip)



Getting started
===============

clone the repo and change into the new directory

run the following 2 commands

#####make build
#####make binary

after successful build the binary will be located in bundles/1.7.1-rc3/binary/

copy your current docker to .old (cp /usr/bin/docker /usr/bin/docker.old)
copy the new version in to place cp bundles/1.7.1-rc3/binary/docker-1.7.1-rc3 /usr/bin/docker

check the version
#####$ docker version
#####Client version: 1.7.1-rc3
#####Client API version: 1.19
#####Go version (client): go1.4.2
#####OS/Arch (client): linux/arm
#####Server version: 1.7.1-rc3
#####Server API version: 1.19
#####Go version (server): go1.4.2
#####Git commit (server):
#####OS/Arch (server): linux/arm

restart the daemon
#####service docker restart
Usage examples
==============

run a container
#####docker run -i -t resin/rpi-raspbian /bin/bash

install nmap in your container
#####apt-get update && apt-get install nmap -y

use your imagination :)

Contributing to Docker
======================

[![GoDoc](https://godoc.org/github.com/docker/docker?status.svg)](https://godoc.org/github.com/docker/docker)
[![Jenkins Build Status](https://jenkins.dockerproject.org/job/Docker%20Master/badge/icon)](https://jenkins.dockerproject.org/job/Docker%20Master/)

Want to hack on Docker? Awesome! We have [instructions to help you get
started contributing code or documentation.](https://docs.docker.com/project/who-written-for/).

These instructions are probably not perfect, please let us know if anything
feels wrong or incomplete. Better yet, submit a PR and improve them yourself.

Licensing
=========
Docker is licensed under the Apache License, Version 2.0. See
[LICENSE](https://github.com/docker/docker/blob/master/LICENSE) for the full
license text.

Other Docker Related Projects
=============================
There are a number of projects under development that are based on Docker's
core technology. These projects expand the tooling built around the
Docker platform to broaden its application and utility.

* [Docker Registry](https://github.com/docker/distribution): Registry 
server for Docker (hosting/delivery of repositories and images)
* [Docker Machine](https://github.com/docker/machine): Machine management 
for a container-centric world
* [Docker Swarm](https://github.com/docker/swarm): A Docker-native clustering 
system
* [Docker Compose](https://github.com/docker/compose) (formerly Fig): 
Define and run multi-container apps
* [Kitematic](https://github.com/kitematic/kitematic): The easiest way to use 
Docker on a Mac

If you know of another project underway that should be listed here, please help 
us keep this list up-to-date by submitting a PR.
