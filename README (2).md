<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Virtual Private Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-vpc)

**Author:** Abhinandan R PAREWA  
**Email:** abhinandan.kr2005@gmail.com

---

## Build a Virtual Private Cloud (VPC)

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-networks-vpc_2facf927)

---

## Introducing Today's Project!

Today we are here to talk about the cloud networking especially about the AWS

### What is Amazon VPC?

Amazon Virtual Private Cloud (VPC) provides a logically isolated, secure, and customizable virtual network within the AWS Cloud, allowing users to define IP address ranges, subnets, route tables, and gateways. It enables launching resources like EC2 instances in a private, segmented environment, with options for public-facing subnets and private, non-internet-facing subnets. 

Today we studied about cloud networks concepts in very detail and also saw how to practically apply them

### Personal reflection

This project took me around 40 minutes

One thing i did not expect was to make an IAM user

---

## Virtual Private Clouds (VPCs)

### What I did in this step

Access the VPC console in AWS.
Create a VPC.



### How VPCs work

VPCs are the reason why resources can be made private to you. You also get control over resources in a VPC, so you can organize how they communicate and integrate with each other without the public internet.



### Why there is a default VPC in AWS accounts

When I created your AWS account, AWS automatically sets up a default VPC .This default VPC is why you could launch resources and connect services together from Day 1 of using AWS. If it didn't exist, you would've had to learn how to create a VPC before you can use some of the services that need VPCs to function.

This default VPC is a handy starting point, especially for beginners, but you can always create custom VPCs to fit specific requirements e.g. strict security measures

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-networks-vpc_2facf927)

### Defining IPv4 CIDR blocks

IPv4 stands for Internet Protocol version 4, which is the most common way to write an IP address. IPv4 address are written as four sets of numbers separated by dots (e.g., 192.168.0.1).



---

## Subnets

### What I did in this step

Launch a subnet inside your VPC.



### Creating and configuring subnets

subnets are like different neighborhoods inside your city. You use subnets to group resources with similar access rules and restrictions. Some subnets might be public areas that all resources can access (public subnets) while others are private areas with limited access (private subnets).

### Public vs private subnets

For example, if you're running a web app, the public-facing website needs to be accessible from the internet - so an EC2 instance hosting the website should be launched in the public subnet.

On the other hand, the web app's database that's storing sensitive data shouldn't be directly accessible from the internet. It only needs to communicate with the EC2 instance, so it can sit in the private subnet.

While your subnet is labeled Public 1, it isn't a public subnet yet. We still need to connect it to an internet gateway to call it public, which you'll attach in a minute.

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-networks-vpc_157c4219)

### Auto-assigning public IPv4 addresses

By default, your resources already have private IP addresss, but this only allows internal communication within your VPC.To access the internet or be accessible from the internet, the instance would need a public IP address.

---

## Internet gateways

### What I did in this step

Connect your VPC to the internet using a internet gateway.



### Setting up internet gateways

An internet gateway connects your city (VPC) and the outside world (internet).

Internet gateways are key to making applications available on the internet. By attaching an internet gateway, your instances can access the internet and be accessible to external users

Attaching an internet gateway means resources in your VPC can now access the internet. The EC2 instances with public IP addresses also become accessible to users, so your applications hosted on those servers become public too

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-networks-vpc_4ae90410)

---

## Using the AWS CLI

### What I'm doing in this extension

### Exploring CloudShell and CLI

### Debugging my setup

### Comparing CloudShell vs AWS Console

---

---
