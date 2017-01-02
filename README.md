# Beginning ASP.NET Web application
Source:  https://github.com/docker/labs/tree/master/windows/aspnet-web#beginning-aspnet-web-application 
But this is for Linux Containers...

The following sample is for Windows Containers.

A simple example using asp.net to serve a web page. First `clone` this repository, and then you can build a new image of your own. 

```

$ git clone https://github.com/kahootali/ASP.Net-App-for-Windows-Containers.git
$ cd ASP.Net-App-for-Windows-Containers/aspnet-web/webserver
$ docker build -t myaspnet .
$ docker run myaspnet
```
Then open up [http://localhost:5000](http://localhost:5000)