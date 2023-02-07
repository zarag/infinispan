FROM azul/zulu-openjdk:11-latest
ADD /target/infinispan-server-12.1.8.Final/. /opt/infinispan
COPY --chown=root ./cluster.xml /opt/infinispan/server/conf/infinispan.xml
COPY --chown=root ./users.properties /opt/infinispan/server/conf/users.properties
ENTRYPOINT ["sh", "/opt/infinispan/bin/server.sh"]
EXPOSE 11222
