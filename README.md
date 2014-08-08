nexus
=====


This repository contains the source for the [Sonatype Nexus](http://www.sonatype.org/nexus) [docker](https://docker.io) image.

# Image details

1. Based on debian:wheezy
1. Supervisor and nexus
1. No SSH.  Use [nsenter](https://github.com/jpetazzo/nsenter)
1. As always, update passwords for pre-installed accounts

# Usage
Start a new container and bind to host's port 8081

```
sudo docker run -p 8081:8081 -t jordan/nexus:latest
```

# Volumes

```
/opt/sonatype-work
/opt/nexus/conf
```
