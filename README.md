# docker-liferay-dxp-wildfly
Docker image for Liferay DXP on Wildfly (JBoss)

See: https://hub.docker.com/r/dorgendubal/liferay-dxp-wildfly/

## Build docker image

docker build -t liferay-dxp-wildfly .

## Run docker image

docker run -it -p 8080:8080 liferay-dxp-wildfly
