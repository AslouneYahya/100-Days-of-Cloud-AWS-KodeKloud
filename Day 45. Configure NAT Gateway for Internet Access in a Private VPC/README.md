# Day 45: Configure NAT Gateway for Internet Access in a Private VPC

I created a new public subnet 
![](45.1.png)

![](45.2.png)

![](45.3.png)

Then, I created a new internet gateway, and I associated it with private vpc

![](45.4.png)

![](45.5.png)

Then I create new public route table, I added my new internet gateway, then I associated it to my public subnet

![](45.6.png)

![](45.7.png)

![](45.8.png)

I created a new NAT Gateway, and I waited until it's on available state

![](45.9.png)

![](45.10.png)

![](45.11.png)

I created a new private route table, then I associated it with private subnet, and I added NAT Gateway to its routes

![](45.13.png)

![](45.14.png)

Finally, the txt file wa uploaded successfully in my s3 bucket.

![](45.15.png)
