# Day 38: Deploying Containerized Applications with Amazon ECS

I created a new ecr 
![](38.1.png)

Then I built my image
![](38.2.png)

I linked docker to my ecr, then I pushed my image
![](38.3.png)

I created a new cluster
![](38.4.png)

Then a new Task definition for my image
![](38.5.png)

![](38.6.png)

Whitin my cluster, I created a new service

![](38.7.png)

![](38.8.png)

I changed inbound rules of default security group, to allow http requests
![](38.9.png)

Using public address of my service, I had access to my nginx server showing this message
![](38.10.png)
