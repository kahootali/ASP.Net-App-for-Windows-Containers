# Beginning ASP.NET Web application for Windows Containers
Source:  https://github.com/docker/labs/tree/master/windows/aspnet-web#beginning-aspnet-web-application 
But this is for Linux Containers...

The following sample is for Windows Containers.

A simple example using asp.net to serve a web page. First `clone` this repository, and then you can build a new image of your own. 

```

$ git clone https://github.com/kahootali/ASP.Net-App-for-Windows-Containers.git
$ cd ASP.Net-App-for-Windows-Containers/webserver
$ docker build -t myaspnet .
$ docker run myaspnet
```
Get the container ID by:
```
docker ps -a
```
Then inspect the IP of the container by :
```
docker inspect -f "{{ .NetworkSettings.Networks.nat.IPAddress }}" <Container-ID>
```

Then open up <container-IP>:5000 in browser