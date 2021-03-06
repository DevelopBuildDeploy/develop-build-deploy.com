---
date: 2018-01-17T16:13:00+01:00
lastmod: 2018-01-17T16:13:00+01:00
title: "Serverless and cost-efficient static website provisioning on AWS S3 & CloudFront using Terraform"
description: 'A reusable infrastructure-as-code approach for quickly provisioning static websites on AWS S3 & CloudFront in a serverless and cost-efficient way, with optional htaccess password protection via Lambda functions, using Terraform'
authors: ["manuelkiessling"]
slug: terraform-automated-cost-efficient-and-serverless-static-site-hosting-aws-s3-cloudfront-lambda-htaccess
draft: true
---

## About

The following describes a reusable infrastructure-as-code approach for quickly provisioning static websites on AWS S3 & CloudFront in a serverless and cost-efficient way, with optional htaccess password protection via Lambda functions, using Terraform.


## Introduction

What's the best way to host a static web site in 2019? Well, one very reliable, scalable, and cost-efficient way that can also be fully automated via an infrastructure-as-code approach is using AWS and Terraform.

This way, we can set up an S3 bucket that contains our HTML, CSS, and JavaScript contents, which are then served through the global AWS content delivery network, CloudFront. We can upload and manage the site's content with any modern file transfer application, and thanks to the AWS infrastructure, we get a website availability of at least 99,9% (according to https://aws.amazon.com/cloudfront/sla/?nc1=h_ls).


## The architecture

The setup we are going to create is relatively simple. Its most important property is that it's completely serverless, which is key to keep costs down even if our site should experience large volumes of visitor traffic. That said, any kind of conventional "back-end application logic" is out of the question; we are not going to deploy any kind of virtual machine or Docker container where we could run



## The terraform setup

```hcl-terraform
```
