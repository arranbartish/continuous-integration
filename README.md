# continuous-integration

# docker hub project

https://hub.docker.com/r/arranbartish/continuous-integration/



```
$ docker build -t continuous-integration .
$ docker run -d --name ci-data continuous-integration echo "data-only container for jenkins"
$ docker run -d -p 8081:8080 --name ci --volumes-from ci-data continuous-integration
$ docker run -p 8081:8081 continuous-integration  
```
