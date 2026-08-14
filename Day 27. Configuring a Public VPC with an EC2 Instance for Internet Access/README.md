# Day 27: Configuring a Public VPC with an EC2 Instance for Internet Access

I created a new vpc

![](27.1.png)

![](27.2.png)

![](27.3.png)

I created a new subnet associated to my new vpc

![](27.4.png)

![](27.5.png)

I enabled auto assign public ipv4 address

![](27.6.png)

![](27.7.png)

![](27.8.png)

I created a new internet gateway, then attached it to my new vpc

![](27.9.png)

![](27.10.png)

![](27.11.png)

I edited my new vpc routing table, to add my internet gateway to it

![](27.12.png)

![](27.13.png)

![](27.14.png)

![](27.15.png)

I verified whether my new subnet is associated to my new vpc's rout table

![](27.16.png)

![](27.17.png)

I created a new ec2 instance with demanded configuration

![](27.18.png)

![](27.19.png)

![](27.20.png)

![](27.21.png)

![](27.22.png)


