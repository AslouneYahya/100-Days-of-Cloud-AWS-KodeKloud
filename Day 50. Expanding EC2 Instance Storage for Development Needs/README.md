# Day 50: Expanding EC2 Instance Storage for Development Needs


I modified my gp3 volume to 12 gb using aws cli, and waited until this modification is completed

![](50.1.png)

![](50.2.png)

I connected to my ec2 instance, then I stratched the partition 1 to fill the remaining 4 gb in the physical xvda disk, then I expanded the XFS filesystem itself.

![](50.3.png)

![](50.4.png)


