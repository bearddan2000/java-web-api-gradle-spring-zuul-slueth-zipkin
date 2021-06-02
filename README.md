# java-web-api-gradle-spring-zuul-slueth-zipkin

## Description
A springboot app that uses zuul
as a reverse proxy. All requests
to `/api` will be forwarded to nodejs
server.

### STEP 1
Once the project is done building, make
some api calls.

### STEP 2
- goto http://localhost
- click on "Find a trace"
  - search by "serviceName"

## Tech stack
- java
- gradle
  - springboot
  - netflix zuul
  - sleuth
  - zipkin
- nodejs

## Docker stack
- gradle:jdk11
- node:latest
- openzipkin/zipkin

## To run
`sudo ./install.sh -u`
- ZIPKIN DASHBOARD http://localhost
- API http://localhost/all
- API remote service http://localhost/api/all

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credits
- https://spring.io/guides/gs/routing-and-filtering/
- https://github.com/openzipkin-attic/docker-zipkin/blob/master/docker-compose.yml
- https://cloud.spring.io/spring-cloud-sleuth/1.3.x/multi/multi__sending_spans_to_zipkin.html
- https://howtodoinjava.com/microservices/spring-cloud-zipkin-sleuth-tutorial/
- https://www.javainuse.com/spring/cloud-sleuth
