# Cloud Resume Challenge 

Introduction
The project involves hosting a static website on Amazon simple storage service (S3) bucket. 
CloudFront was be used for distribution. SSL/TLS from AWS Certificate Manager is used for 
secure access to the Amazon S3 bucket. Amazon Route 53 was used for domain naming. CloudFormation 
will be used for deployment.                                                                                           

Step-by-step guidelines

Amazon Simple Storage Service configuration
1. Creation of an S3 bucket that hosts the static cloud resume website.
2.

Cloud Front configuration
1. Creation of CloudFront distribution to serve the website to users over the internet.

ACM Configuration
1. Creation of an SSL/TLS certificate in ACM, and attaching it to the CloudFront distribution.
    This enables the distribution to serve the domain’s website using HTTPS.

Aquiring a Domain Name 

Using Route53 for Domain Naming

Architectural Diagram  

1. The viewer requests the website at www.example.com.
2. If the requested object is cached, CloudFront returns the object from its cache to the viewer.
3. If the object is not in CloudFront’s cache, CloudFront requests the object from the origin (an S3 bucket).
4. S3 returns the object to CloudFront
5. CloudFront caches the object.
6. The object is returned to the viewer. Subsequent responses for the object are served from the CloudFront cache.

Project Challenges
Time constraints
Limited Knowledge of HTML and CSS

Key Takeaways
I can turn my fears into something beneficial


Resources
https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html
https://docs.aws.amazon.com/acm/latest/userguide/acm-services.html
https://github.com/aws-samples/amazon-cloudfront-secure-static-site
https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html
https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-configuring-new-domain.html



