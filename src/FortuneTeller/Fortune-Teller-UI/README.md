## Fortune-Teller-UI

Features demonstarted 

* Config server
* Discovery client
* Redis Server
* Health management
* Hystrix (in-progress)



 ## Required nuget packages

Microsoft.Extensions.Hosting  
Microsoft.Extensions.Logging.Console  
Unity.Aspnet.Webapi   
Unity.Microsoft.DependencyInjection  

Pivotal.Extensions.Configuration.ConfigServercore  
Pivotal.Discovery.ClientCore  
Steeltoe.Management.EndpointWeb  
Steeltoe.CloudFoundry.Connectorcore  

StackExchange.Redis  
Steeltoe.CircuitBreaker.HystrixCore  



## endpoints to test 

<YOUR_PCF_APP_URL>/home/random
<YOUR_PCF_APP_URL>/home/cached


## Building and Running the app

Conncted services:
coreConfigServer    -   config server service
redisInstance       -   redis service 
eurekaServer        -   service registry service
hystrixService      -   circuit breaker service

## Things in progress
Could not get the HystrixCommand to work. Commented out code blocks. Will revist it.