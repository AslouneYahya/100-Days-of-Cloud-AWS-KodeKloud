# Day 29: Establishing Secure Communication Between Public and Private VPCs via VPC Peering

I created a new peering connection between default vpc and my private one

![](29.1.png)

![](29.2.png)

![](29.3.png)

![](29.4.png)

![](29.5.png)

I added it to route tables for both VPCs

![](29.6.png)

![](29.7.png)

![](29.8.png)

![](29.9.png)

I changed security rules for security groups of both ec2 instances; I added ssh inbound rule for public ec2 instance, and icmp for private ec2 instance

![](29.10.png)

![](29.11.png)

![](29.12.png)

![](29.13.png)

![](29.14.png)

To establish ssh connection, I copied my aws-client public key to my public ec2 instance ~/.ssh/authorized_keys file

![](29.15.png)

![](29.16.png)

![](29.17.png)

![](29.18.png)

I was able to make a ssh connection to public ec2 instance, and I was able to ping my private ec2 instance from public one using private ipv4 address of my private ec2 instance

![](29.19.png)

![](29.20.png)


