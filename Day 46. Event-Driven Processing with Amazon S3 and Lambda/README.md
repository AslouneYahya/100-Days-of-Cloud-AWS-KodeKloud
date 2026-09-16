# Day 46: Event-Driven Processing with Amazon S3 and Lambda

I created a public and a private s3 buckets
![](46.1.png)

![](46.2.png)

![](46.3.png)

![](46.4.png)

![](46.5.png)

![](46.6.png)

then, I created my DynamoDB to store logs of my lambda function

![](46.7.png)

![](46.8.png)

I created a IAM role wuth proper policies to associate it with my lambda function

![](46.9.png)

![](46.10.png)

![](46.11.png)

![](46.12.png)

then, I copied the python script in aws-client

![](46.13.png)

After that, I created my lambda function with proper configuration

![](46.14.png)

![](46.15.png)

![](46.16.png)

![](46.17.png)

![](46.18.png)

then, I uploaded my zip file to my public s3 bucket, then I verified changes in private s3 bucket, and my DynamoDB

![](46.19.png)

![](46.20.png)

![](46.21.png)
