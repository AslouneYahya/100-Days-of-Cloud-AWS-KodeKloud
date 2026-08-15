# Day 30: Enable Internet Access for Private EC2 using NAT Instance

I created a new public subnet in my private vpc, then enabled auto-assign public ipv4 address in it

![](30.1.png)

![](30.2.png)

![](30.3.png)

![](30.4.png)

![](30.5.png)

I created a new internet gayeway then I attached it to my private vpc

![](30.6.png)

![](30.7.png)

![](30.8.png)

![](30.9.png)

I created a new route table in my private vpc, then I added my newky created internet gateway to it, then I associated it to my public subnet

![](30.10.png)

![](30.11.png)

![](30.12.png)

![](30.13.png)

![](30.14.png)

![](30.15.png)

I created a new security group that allows all inbound traffic from my private ec2 instance, and ssh from all sources, then I created my nat instance, then I stopped checking source/destination in it

![](30.16.png)

![](30.17.png)

![](30.18.png)

![](30.19.png)

![](30.20.png)


![](30.21.png)

![](30.22.png)

![](30.23.png)

![](30.24.png)

I changed iptables configuration in my nat instance to enable forwarding and masquerading packets from my private instance

![](30.25.png)

![](30.26.png)

![](30.27.png)

![](30.28.png)

![](30.29.png)

I changed routes of my private subnet to forward requests to my nat instance

![](30.30.png)

![](30.31.png)

![](30.32.png)

Here I reconfigured my nat instance to use the correct network interface name

![](30.33.png)

I verified that my s3 bucket contains the txt file, uploaded by my private instance using my nat instance as a gateway

![](30.34.png)

![](30.35.png)