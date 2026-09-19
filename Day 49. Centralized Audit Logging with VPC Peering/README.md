# Day 49: Centralized Audit Logging with VPC Peering

I created a new public vpc, public subnet, internet gateway for my public vpc, and a route table for my public subnet

![](49.1.png)

![](49.2.png)

![](49.3.png)

![](49.4.png)

![](49.5.png)

![](49.6.png)

![](49.7.png)

![](49.8.png)

I lunched an ec2 instance in public subnet, then I associated an iam role so it could post files in s3 buckets

![](49.9.png)

![](49.10.png)

![](49.11.png)

![](49.12.png)

![](49.13.png)

![](49.14.png)

![](49.15.png)

I created a s3 bucket, to post logs from public ec2 instance to it

![](49.16.png)

![](49.17.png)

I created a peering connection between my private vpc and my public vpc, then I added it to public route table, and private route table

![](49.18.png)

![](49.19.png)

![](49.20.png)

![](49.21.png)

I tested ssh connection using my aws-client machine, then I generated public and private ssh keys in my private ec2 instance, then I copied it, and added it to authorized_keys file in public ec2 instance

![](49.22.png)

![](49.23.png)

![](49.24.png)

![](49.25.png)

I created two cron jobs, one in my private ec2 instance, to send logs to my public instance, and the other one in my public ec2 instance to send the recieved logs to my s3 bucket

![](49.26.png)

![](49.27.png)

![](49.28.png)

![](49.29.png)

![](49.30.png)

![](49.31.png)

![](49.32.png)

after this, the logs should appear in s3 bucket.