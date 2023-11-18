## Deploying a Static Website on S3 and disploys a CloudFront.

####  This is a demo project where I delpoyed a fullstack(Frontend + backend) app on AWS using their resources.  It uses an Amazon S3 bucket for file storage, configures the bucket to host a website, and deploys an Amazon CloudFront Distribution to serve the website with low latency, caching, and HTTPS.

#### Resources used in this project:
- S3 
- CloudFront

#### tech I hacve Used:
- HTML
- CSS
- JAVASCRIPT
- BACKTRACKING
### Project Architecture:


### What I did:

Firstly, I developed a website that efficiently solves any given Sudoku problem using the backtracking algorithm, implemented in JavaScript. Subsequently, I accessed the AWS console to create an S3 Bucket, naming it "aaravbagla-sudoku" and configuring it with default settings.

Upon creating the S3 bucket, I uploaded all the necessary files for the Sudoku application, including index.js, style.css, and script.js. Moving forward, I navigated to S3 permissions and enabled the bucket for static website hosting.

Continuing the setup, I logged into CloudFront and generated a distribution for my S3 bucket, specifying index.js as the origin, and restricting access to the S3 traffic exclusively through CloudFront. Following the creation of the distribution, I updated the S3 bucket policy to allow traffic only to this specific CloudFront distribution.

With these configurations in place, the website is now accessible across AWS Edge Locations, providing users with low-latency access to the Sudoku-solving application.