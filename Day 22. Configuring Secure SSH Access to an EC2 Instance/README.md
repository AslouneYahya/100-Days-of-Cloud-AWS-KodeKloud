# Day 22: Configuring Secure SSH Access to an EC2 Instance

After logging in, I searched for EC2 section,

![](22.1.png)

I went for instances section, and I created my new EC2 instance

![](22.2.png)

![](22.3.png)

![](22.4.png)

![](22.5.png)

I generated my ssh key pair in client machine, then copied my generated public key

![](22.6.png)

I connected to my new EC2 instance

![](22.7.png)

I added my copied public key from client machine to  /root/.ssh/authorized_keys file in my server

![](22.8.png)

![](22.9.png)

I fixed the permissions for my directory and file of ssh keys for security measures

![](22.10.png)

Finally, using my generated ssh key pair, I did a ssh connection to my ec2 instance from my client machine

![](22.11.png)
