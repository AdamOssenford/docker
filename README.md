Docker 1.7.1 Fork for Raspberry Pi
==================================

![Docker L](docs/static_files/docker-logo-compressed.png "Docker")

This is a fork of the docker 1.7.1 rc3 build.  The Dockerfile has been modified to compile on a Raspberry Pi2.  Various Pi  package dependencies are required to successfully build.  Hopefully a list of those will make it to this readme in the future

Getting started
===============

clone the repo and change into the new directory

run the following 2 commands
make build
make binary

Usage examples
==============

start the daemon

service docker start

run a container
docker run -it hypriot/rpi-busybox-httpd

Contributing to Docker
======================

[![GoDoc](https://godoc.org/github.com/docker/docker?status.svg)](https://godoc.org/github.com/docker/docker)
[![Jenkins Build Status](https://jenkins.dockerproject.org/job/Docker%20Master/badge/icon)](https://jenkins.dockerproject.org/job/Docker%20Master/)

Want to hack on Docker? Awesome! We have [instructions to help you get
started contributing code or documentation.](https://docs.docker.com/project/who-written-for/).

These instructions are probably not perfect, please let us know if anything
feels wrong or incomplete. Better yet, submit a PR and improve them yourself.

### Legal

*Brought to you courtesy of our legal counsel. For more context,
please see the [NOTICE](https://github.com/docker/docker/blob/master/NOTICE) document in this repo.*

Use and transfer of Docker may be subject to certain restrictions by the
United States and other governments.

It is your responsibility to ensure that your use and/or transfer does not
violate applicable laws.

For more information, please see https://www.bis.doc.gov


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
