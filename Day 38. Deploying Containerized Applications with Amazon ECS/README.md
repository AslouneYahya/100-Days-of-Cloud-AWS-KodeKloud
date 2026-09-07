# Day 37: Managing EC2 Access with S3 Role-based Permissions

I created a ssh connection with my ec2 instance
![](37.1.png)

![](37.2.png)

![](37.3.png)

![](37.4.png)

I connected tomy ec2 instance, then I added my public key to /root/.ssh/authorized_keys in my ec2 instance

![](37.5.png)

![](37.6.png)

I created a new s3 bucket, a new iam policy and role associated with it, then I attached that role to my ec2 instance

![](37.7.png)

![](37.8.png)

![](37.9.png)

![](37.10.png)

![](37.11.png)

![](37.12.png)

![](37.13.png)

![](37.14.png)

![](37.15.png)

![](37.16.png)

![](37.17.png)

![](37.18.png)

HereI modified my role permissions, because I couldn't upload a file, from my ec2 instance to my s3 bucket

![](37.19.png)

At this point, the one hour of my lab was over, I had to redo it again, so I redid all the steps, with the correct permissions, then I uploaded test file successfully

![](37.20.png)
