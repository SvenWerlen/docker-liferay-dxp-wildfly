##
## Docker image: Liferay DXP -> WildFly (JBoss)
## * Languages: fr_CA/en_CA
## * Database: PostgreSQL
##
## Build: docker build -t liferay-dxp-wildfly-quebec .
## Run: docker run -it -p 8080:8080 liferay-dxp-wildfly-quebec
##
FROM dorgendubal/liferay-dxp-wildfly:latest 

# PATHS
ENV LIFERAY_HOME		/opt/app/liferay/
ENV WILDFLY_HOME		/opt/app/liferay/wildfly

COPY files /tmp/files

# INSTALLATION PostgreSQL
USER root
RUN cp /tmp/files/portal-ext.properties $LIFERAY_HOME/ \
   && cp /tmp/files/system-ext.properties $WILDFLY_HOME/standalone/deployments/ROOT.war/WEB-INF/classes/

