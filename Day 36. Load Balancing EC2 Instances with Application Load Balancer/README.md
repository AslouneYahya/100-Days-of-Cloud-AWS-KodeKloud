# Day 36: Load Balancing EC2 Instances with Application Load Balancer

I created a new security group for my ec2 instance

![](36.1.png)

![](36.2.png)

![](36.3.png)

Then, I created my ec2 instance with demanded configuration

![](36.4.png)

![](36.5.png)

![](36.6.png)

![](36.7.png)

Then, I created a new target group, that includes my ec2 instance

![](36.8.png)

![](36.9.png)

![](36.10.png)

![](36.11.png)

After that, I created my new application load balancer, for my target group (ensure that your application load balancer is in the availability zone of your ec2 instance), and I changed inbound rules of default security group to accept http requests

![](36.12.png)

![](36.13.png)

![](36.14.png)

![](36.15.png)

![](36.16.png)

After waiting for some minutes, my target group status went healthy, which means my load balancing setup was successful.

![](36.17.png)
