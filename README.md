# AWS Cognito with Google Identity Provider

This project demonstrates how to integrate AWS Cognito with Google as an Identity Provider (IdP) to authenticate users and provide them with temporary AWS credentials.

## Overview

- **Google API Identity Provider**: Users are directed to Google for authentication.
- **AWS Cognito**: Swaps the Google token for AWS credentials.
- **IAM Role**: Cognito assumes an IAM role to generate temporary AWS credentials.
- **S3 Bucket**: HTML and JavaScript files are loaded from an S3 bucket via CloudFront.
- **Private Objects**: AWS credentials are used to access private objects in the S3 bucket.

## Prerequisites

- AWS Account
- Google Developer Account
- Node.js (if using AWS SDK)

## Setup

1. **Google API Setup**:
   - Create a project in the Google Developer Console.
   - Configure OAuth 2.0 credentials.
   - Set up the consent screen.

2. **AWS Cognito Setup**:
   - Create a Cognito Identity Pool.
   - Configure Google as an Identity Provider.
   - Set up IAM roles for authenticated and unauthenticated users.

3. **S3 Bucket Setup**:
   - Create an S3 bucket.
   - Configure CloudFront as a CDN.
   - Set bucket policies to restrict access.

4. **Deploy**:
   - Upload your HTML and JavaScript files to the S3 bucket.
   - Configure your application to use the Cognito Identity Pool.

