# base image 
This is the base image.
It contains no configuration (everything is Liferay's default).

See: https://hub.docker.com/r/dorgendubal/liferay-dxp-wildfly/

## Build docker image

docker build -t liferay-dxp-wildfly .

## Run docker image

docker run -it -p 8080:8080 liferay-dxp-wildfly
