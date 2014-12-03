# docker debian

* based on offical docker debian
* Add support of supervisor to manage process - add your *.conf files into /etc/supervisor/
* Python installed

## Sample Usage

for running debian latest :

	docker run -i -t studioetrange/docker-debian:latest bash

for running debian wheezy :

	docker run -i -t studioetrange/docker-debian:wheezy bash

## Instruction 

### build from github source

	git pull https://github.com/StudioEtrange/docker-debian
	cd docker-debian
	docker build -t=studioetrange/docker-debian .

### retrieve image from docker registry

	docker pull studioetrange/docker-debian

### run a shell 

	docker run -p SUPERVISOR_HTTP_WEB:9999 studioetrange/docker-debian:DEBIAN_VERSION bash

## Access point

### Supervisor

	Go to http://localhost:SUPERVISOR_HTTP_WEB/
