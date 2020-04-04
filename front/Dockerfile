FROM node
RUN npm install http-server -g

EXPOSE 8084
ARG BACK_HOST
ARG BACK_PORT

RUN mkdir /home/front
WORKDIR /home/front
COPY front.zip .
RUN unzip front.zip

CMD http-server -p 8084 -P http://$BACK_HOST:$BACK_PORT/
