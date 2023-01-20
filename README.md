# EC2 Web-Server

## Goal
Obtain an understanding of how to deploy and maintain a web server through an AWS EC2 instance on Apache.

## Contents
### Summary
The contents of the web-server will progress as I progress in HTML, CSS, and Javascript. The goal is to make a porfolio website.

### Tasks
* [x] Get an EC2 Instance Running
* [x] Get a Basic HTML Web Server Running
* [ ] Apply CSS Styling
* [ ] Basic Portfolio Website

### Public DNS IPv4

For anyone who wants to see the live EC2 instance, click [here](http://www.ec2-54-149-25-154.us-west-2.compute.amazonaws.com).

### User Data
```
#!/bin/bash
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
cd /var/www/html/
```
