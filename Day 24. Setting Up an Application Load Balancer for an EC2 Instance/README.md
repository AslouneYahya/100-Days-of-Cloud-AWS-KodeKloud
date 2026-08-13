# Day 24: Setting Up an Application Load Balancer for an EC2 Instance

After logging in, I searched for EC2 section,

![](24.1.png)

I went for security groups, and I created my new security group

![](24.2.png)

![](24.3.png)

![](24.4.png)

Then I went to target groups, and I created my new target group taht includes my ec2 instance

![](24.5.png)

![](24.6.png)

![](24.7.png)

![](24.8.png)

![](24.9.png)

Then I created my new application load balancer with my security group and target group that I already created 

![](24.10.png)

![](24.11.png)

![](24.12.png)

![](24.13.png)

![](24.14.png)

![](24.15.png)

Then, I reconfigured default security group of my ec2 instance with changing its inbound rule to accept only hhtp request from my newly created security group

![](24.16.png)

![](24.17.png)

![](24.18.png)

![](24.19.png)
