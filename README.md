# Terraform Interview

## Overview

Welcome to your coding interview! In this challenge, you will be tasked with provisioning AWS infrastructure using Terraform. You will set up an ECS (Elastic Container Service) web server.

A 1password share link will be shared with you with relevant AWS access key information

## AWS provider

You are required here to initialize Terraform and the AWS provider.

## Deploy a Single Server

You are required here to provision a single EC2 server.

## Deploy a Web Server

You are required here to extend the EC2 instance to execute the below web server script upon initialization of the EC2 instance:

```sh
#!/bin/bash
apt-get update -y
apt-get install -y apache2
systemctl start apache2
systemctl enable apache2
echo 'Hello World' > /var/www/html/index.html
```

The server is also to be made publically accessible.

Bonus:

Output the public IP as part of the Terraform run.

## Deploy a Configurable Web Server

Using your discretion, further parametrize your Terraform script.

