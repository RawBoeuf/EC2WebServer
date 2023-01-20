# EC2 Web-Server
## Summary
This is my first time using AWS. I've helped out with a website previously, but this is the first time making my own without help. The contents of the web-server will improve as I progress in HTML, CSS, and Javascript. The goal is to make a porfolio website with a basic HTML framework then add some CSS and Javascript.

## Goal
Obtain an understanding of how to deploy and maintain a web server through an AWS EC2 instance on Apache.

## Contents

### Public DNS IPv4

For anyone who wants to see the live EC2 instance, click [here](http://ec2-54-149-25-154.us-west-2.compute.amazonaws.com).

### Tasks
* [x] Get an EC2 Instance Running
* [x] Get a Basic HTML Web Server Running
* [ ] Apply CSS Styling
* [ ] Basic Portfolio Website

### User Data
**This is the user data that I had for my EC2 instance at launch.**
```
#!/bin/bash
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
cd /var/www/html/
echo "Hello, world!" > index.html
```

### Learning Tools Used
#### Paid
* ["Amazon Elastic Compute Cloud (EC2) Beginners Certification" Udemy Course by YouAccel](https://www.udemy.com/share/105nzg3@LMUCniwnz79Iz1TTyOcdvDsecSxWE71Oh-1MaSo5RD51toyK8gsXayz2LP08fpTi/)
#### Free
* ["Markdown Crash Course" by Traversy Media](https://www.youtube.com/watch?v=HUBNt18RFbo)

### StackOverflow and SuperUser Threads Used
* **Purpose:** Used as reference for a bash script that pulls new data from the github repository on startup. [here](https://stackoverflow.com/questions/60072643/how-to-automatically-start-execute-and-stop-ec2)
