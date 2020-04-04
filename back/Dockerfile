FROM java

VOLUME /root/db
EXPOSE 8080
ARG EMAIL
ARG PASS

ADD rest-1.0.jar .
CMD java -jar rest-1.0.jar $EMAIL $PASS
