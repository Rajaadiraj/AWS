<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Cloud Security with AWS IAM

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-security-iam)

**Author:** Abhinandan R PAREWA  
**Email:** abhinandan.kr2005@gmail.com

---

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_1c864649)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate. about IAM users

### Tools and concepts

The key services that we used were making Ec2 instances and iam user and making policy .

### Project reflection

It took me around 1 hr to finish the project

---

## Tags

### What I did in this step

Launch two Amazon EC2 instances so that we can increase NextWork's computing power.

### Understanding tags

Tags are there for tell us what is it for.

### My tag configuration

the tags that we have assigned are development , production,

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_2e0e5a5d)

---

## IAM Policies

### What I did in this step

Create an IAM policy that gives access to the development instance.

### Understanding IAM policies

IAM stands for Identity and Access Management. You'll use AWS IAM to manage the access level that other users and services have to your resources.



### The policy I set up

For this project, I’ve set up a policy using JSON

### Policy effect

This policy allows some actions (like starting, stopping, and describing EC2 instances) for instances tagged with "Env = development" while denying the ability to create or delete tags for all instances

### Understanding Effect, Action, and Resource

This can have two values - either Allow or Deny - to indicate whether the policy allows or denies a certain action. Deny has priority. Looking at the first statement, "Effect": "Allow" means this statement is trying to allow for an action


---

## My JSON Policy

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_1c864649)

---

## Account Alias

### What I did in this step

Simplify user login to your AWS account using an Account Alias.

### Understanding account aliases

An account alias is when different users log into my account they don't login into my main account rather use an alias

### Setting up my account alias

Creating an account alias took me less than 1 minute

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_0eb4439b)

---

## IAM Users and User Groups

### What I did in this step

Set up a dedicated IAM group for all NextWork interns, so you can manage all interns' permissions from one place.

Set up a dedicated IAM user for your new intern, so they have a way to log in.

### Understanding user groups

IAM users are the people that will get access to your resources/AWS account, whereas user groups are the collections/folders of users for easier user management.

We're adding users to nextwork-dev-group to grant them the permissions associated with that group.



### Attaching policies to user groups

I attached the policy so that i know what people will do or not do

### Understanding IAM users

IAM users are IAM users are the people that will get access to your resources/AWS account, whereas user groups are the collections/folders of users for easier user management.



---

## Logging in as an IAM User

### Sharing sign-in details

The first way is 

### Observations from the IAM user dashboard

I noticed it as a new account created .

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_6f2ab446)

---

## Testing IAM Policies

### What I did in this step

Log into AWS using the intern's IAM user.
Test the intern's access to your production and development instance.

### Testing policy actions

I tested my JSON IAM policy by, we created two instances of different types.

### Stopping the production instance

When I tried to stop the production instance it showed me error as i can not do.

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_0e7a9d6a)

### Stopping the development instance

when we tried to stop the development instance it did not stop as iam user did not have permission

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-security-iam_1811801c)

---

## IAM Policy Simulator

### Understanding the IAM Policy Simulator

### How I used the simulator

---

---
