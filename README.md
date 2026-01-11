# Static Website Hosting on AWS

This project demonstrates how to host a secure, scalable static website on AWS.

## Architecture Diagram
![Static Website Architecture](static-website-cloudfront-distribution.png)

## Services Used
- Amazon S3 (static website hosting)
- Amazon CloudFront (CDN and HTTPS termination)
- Amazon Route 53 (DNS)
- AWS Certificate Manager (TLS/SSL)

## Architecture Flow
1. User performs a DNS lookup via Route 53.
2. CloudFront serves the website over HTTPS.
3. On cache miss, CloudFront fetches content from S3.
4. Content is cached at edge locations and returned to the user securely.

## Outcome
- Secure HTTPS website
- Global content delivery
- Low-latency access
- AWS-managed scalability
