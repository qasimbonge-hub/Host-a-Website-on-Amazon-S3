<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](https://nextwork.ai/projects/70e2d059-31ab-5f67-8c58-f5edbd451140)

**Author:** Asimbonge Qwabe  
**Email:** qasimbonge@gmail.com

---

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_5d4474f9)

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate how to host a Website on Amazon S3. I'm doing this project to learn the fundamentals of S3

### Tools and concepts

Services I used were Amazon S3. Key concepts I learnt include ACLs, static website hosting, bucket website endpoint and bucket policy

### Time, challenges, and wins

This project took me approximately 30 minutes. The most challenging part was adding a bucket policy. It was most rewarding to make the objects in the S3 public

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will open S3 because I will create a storage space for my website files

### How long it took to create the bucket

Creating an S3 bucket took me less than 2 minutes

### Region selection

The Region I picked for my S3 bucket was Cape Town because it is the closest region to me

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means no other AWS account in the entire world can use my bucket's name unless I delete it

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_ba6d42ad)

## Upload Website Files to S3

### What I did in this step

In this step, I will upload an HTML file and a zip file because both of those files contain data and images to set up the website

### Files I uploaded

I uploaded two files to my S3 bucket - they were an HTML file and an index file 

### How the files work together

Both files are necessary for this project as a way to display the website with a setup and images

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_a265af88)

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure a static website on Amazon S3 because I want to visit the public website link

### Understanding website hosting

Website hosting means what makes your website public on the internet

### How I enabled website hosting

To enable website hosting with my S3 bucket, I edited the static website hosting to enable it, chose to host a static website, and entered the index.html files that are already uploaded in the bucket

### Access Control Lists (ACLs)

An ACL is a set of rules that decides who can get access to a resource. I enabled the ACLs

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_c22c54c0)

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is it lets people visit the S3 bucket's files as a website

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw a 403 error. The reason for this error was that objects such as the index.html file were still private when it was uploaded

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_22ce4daf)

## Success!

### What I did in this step

In this step, I will make the objects in the S3 bucket public because the website can be live on the internet with no errors

### How I resolved the 403 error

To resolve this 403 Forbidden error, I selected the checkboxes next to the index.html file and the folder under the objects tab, went through actions and made public using ACL

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_5d4474f9)

## Bucket Policies

### What I did in this extension

In this project extension, I'm about to set up a bucket policy and test that policy. I'm doing this so that it stops people from deleting the index.html file

### Understanding bucket policies

An alternative to ACLs are bucket policies, which control access by matching a request against several conditions. The benefit of using bucket policies is that whenever anyone tries to delete an object from this bucket, AWS evaluates security in a specific sequence, while ACLs are useful for allowing a user to read or write

![Image](https://nextwork.ai/mindful_olive_jolly_dragonfly/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_sm2sm2sm)

### What my bucket policy does

My bucket policy denies access to delete the file. I tested this by deleting an index.html file and saw that my access was denied

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/70e2d059-31ab-5f67-8c58-f5edbd451140)*
