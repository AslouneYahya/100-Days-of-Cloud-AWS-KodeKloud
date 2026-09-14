# Day 44: Implementing Auto Scaling for High Availability in AWS


I created a new security group that allows inbound http resquests

![](44.1.png)

![](44.2.png)

Then, I created a new ec2 lunch template with demanded configuration

![](44.3.png)

![](44.4.png)

![](44.5.png)

![](44.6.png)

![](44.7.png)

After that, I crated a new target group

![](44.8.png)

![](44.9.png)

Then, a new application load balancer for my target group

![](44.10.png)

![](44.11.png)

![](44.12.png)

Then, I created my auto scaling group with demanded configuration

![](44.13.png)

![](44.14.png)

![](44.15.png)

![](44.16.png)

![](44.17.png)

![](44.18.png)

Finally my instance is accessible using its dns public address

![](44.19.png)
