# ASP.NET 4.x Sample Applications with Unity and Steeltoe 

This repo contains sample apps illustrating how to use the Steeltoe libraries for connecting to CloudFoundry services in your ASP.NET 4.x application. These sample apps use Unity DI. It takes quite an effort to instrument full framework app to use Steeltoe features. Autofac extensions are available for full framework to abstarct away that effort. But there are no Unity extensions availble. 

The concept is pretty simple- configure and add services to Micorsoft DI and load them into Unity container. So you can use Unity for your apps the same way you do and can inject Steeltoe interfaces (Unity container can resolbve them). 


## ASP.NET 4.x Samples

* src/ScratchPad/SteeltoeUnityIoC - sample application to demonstarte loading service registartions from Microsoft DI container to Unity container
* src/FortuneTeller/Fortune-Teller-Service - use config server, connect to a MS SQL database on Azure, use Discovery client, add health management
* src/FortuneTeller/Fortune-Teller-UI - use config server, connect to Fortune-Teller-Service using Discovery client, add health management, connect to Redis server on CloudFoundry
