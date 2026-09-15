# AWS-Hosted CV 

## Project Overview

This project hosts my professional CV on Amazon Web Services (AWS) using a secure cloud-based architecture.

The CV is stored in a private Amazon S3 bucket and delivered to users through Amazon CloudFront over HTTPS.

## Architecture

User
|
Amazon CloudFront
|
Private Amazon S3 Bucket
|
CV PDF

## AWS Services Used

- Amazon S3
- Amazon CloudFront
- AWS WAF

## Implementation

### Amazon S3

The CV PDF is stored in an Amazon S3 general-purpose bucket.

The bucket is configured with:

- Block Public Access enabled
- ACLs disabled
- Bucket versioning enabled
- Server-side encryption using S3-managed keys
- Private object storage

### Amazon CloudFront

Amazon CloudFront is used to deliver the CV through HTTPS while keeping the S3 bucket private.

CloudFront uses secure access to retrieve the CV from the S3 bucket.

### AWS WAF

AWS WAF is enabled on the CloudFront distribution to provide an additional web-application security layer.

## Project Goal

The purpose of this project is to gain practical experience designing and deploying a secure AWS-based solution while creating a publicly accessible version of my professional CV.

## Skills Demonstrated

- Amazon S3
- Amazon CloudFront
- AWS WAF
- Cloud security
- Object storage
- HTTPS content delivery
- AWS access control
- Cloud architecture
