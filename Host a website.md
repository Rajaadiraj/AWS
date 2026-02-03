<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** Abhinandan R PAREWA  
**Email:** abhinandan.kr2005@gmail.com

---

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project we are going to learn how to use AWS services and one of the services that we are going to learn is to host a website on AWS.

### Tools and concepts

The key services that we used were the AWS S3 , in it we learned how to host a website and we also learned about bucket policy

### Time, challenges, and wins

It took me about 1 hr to finish the project

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will open the Amazon S3 services to make a storage space for the website that we are going to host.

### How long it took to create the bucket

Creating an S3 bucket took me about 5 minutes to create

### Region selection

The Region I picked for my S3 bucket was Mumbai (asia) as it is the closest to me.

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means that with the name I created for the bucket, i will only be able to use it.

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

Download an HTML file that sets up your website.

Download a zip file of images for your website.

Upload both files into your S3 bucket

### Files I uploaded

I uploaded two files to my S3 bucket - they were an Index.html file and the other was an unzipped folder.

### How the files work together

Both files are necessary for this project as it would have content of file to the other

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step we will
Configure your S3 bucket for static website hosting

Visit your public website link

### Understanding website hosting

Website hosting means making our website public to the internet.

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went to properties and then all the way down and enable static web hosting in it.

### Access Control Lists (ACLs)

An ACL is a set of rules that decides who can get access to a resource.

Enabling ACLs in this S3 setup lets you control who can access and do things with the objects you upload into your bucket.

With ACLs, different AWS accounts can own and control different files in your 

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is http://nextwork-website-project-abhinandan.s3-website.ap-south-1.amazonaws.com/

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw... The reason for this error was as my contents are private and we want to make it public.

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

Make your website files in S3 publicly accessible.

See your website live on the internet

### How I resolved the 403 error

To resolve this 403 Forbidden error, I did not got this error.

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this mission we are checking who can delete and who cannot by objects in the S3

### Understanding bucket policies

In bucket policy we are telling the cloud who has some controls , permission and what so ever

![Image](http://learn.nextwork.org/triumphant_turquoise_silly_rose_apple/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy is way to tell people about the who has the control over the buckets . In bucket policy we can create different types of policy like the delete and from the above we are letting anyone delete our objects bucket.

---

---
