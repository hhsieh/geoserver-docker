# geoserver-docker

[GeoServer](http://geoserver.org) is an open source server for sharing geospatial data.
This is a modified docker image based on
https://github.com/GeoNode/geoserver-docker and modified to work with a remote
JNDI ssl connection

The image is based on the official Tomcat 9 image

## Quick start

```bash
$ git clone https://github.com/kf8a/geoserver-docker.git
$ cd geoserver-docker
$ cp context.xml.example context.xml
```

Customize context.xml

```bash
$ docker build -t "geonode/geoserver" .
```

Build the data-docker image as in https://github.com/GeoNode/data-docker

```bash
$ docker-compose up
```

Point your browser to `http://localhost:8080/geoserver` and login using GeoServer's default username and password:

* Username: admin
* Password: geoserver

