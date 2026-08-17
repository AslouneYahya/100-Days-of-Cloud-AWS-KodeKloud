# Day 35: Deploying and Managing Applications on AWS

I created a new rds instance with demanded configuration

![](35.1.png)

![](35.2.png)

![](35.3.png)

![](35.4.png)

![](35.5.png)

![](35.6.png)

![](35.7.png)

![](35.8.png)

I change inbound rules of my ec2 instance's security group to allow http and ssh requests 

![](35.9.png)

![](35.10.png)

![](35.11.png)

I created a passwordless connection between aws-client and my ec2 instance

![](35.12.png)

![](35.13.png)

![](35.14.png)

![](35.15.png)

![](35.16.png)

I copied index.php file from aws-client to my ec2 instance, then I changed its database credentials with my newly created database

![](35.17.png)

![](35.18.png)

![](35.19.png)

After saving the changes, I did a curl request to localhost, which showed that my database is connected successfully to my ec2 instance

![](35.20.png)
