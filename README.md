Portfolio Website Hosted on AWS S3
This repository contains the source code for a personal portfolio website hosted on AWS S3. The project demonstrates how to create, configure, and deploy a static website using Amazon S3, ensuring high availability, scalability, and cost-effectiveness.

Features
Responsive Design: Built with HTML, CSS, and JavaScript to provide a seamless user experience across devices.
Fast and Secure Hosting: Deployed on AWS S3 with optional CloudFront CDN for enhanced performance and HTTPS support.
Easy Deployment: Includes scripts or guidelines to update and deploy changes quickly.
Custom Domain: Supports integration with a custom domain and HTTPS using AWS Certificate Manager.

Technologies Used

Frontend: HTML5, CSS3, JavaScript
Hosting: AWS S3 for static site hosting.
Optional Add-ons:
AWS CloudFront for content delivery.
AWS Route 53 for domain management.
AWS Certificate Manager for SSL/TLS.

Prerequisites
To run or deploy this project, you need:

An AWS account with access to S3.
A domain name (optional, for custom domain setup).
AWS CLI (Command Line Interface) configured on your local machine.

Getting Started
Clone the Repository

git clone https://github.com/Devkhuman/Portfolio-aws-s3.git
cd Portfolio-aws-s3

Setup
Modify Content: Update the HTML, CSS, and JavaScript files in the src/ directory to personalize your portfolio.
Test Locally: Use a local HTTP server to preview your site. For example:

python3 -m http.server
Then, visit http://localhost:8000 in your browser.

Deployment
Create an S3 Bucket:

Log in to your AWS Management Console.
Create an S3 bucket (e.g., your-portfolio-bucket).
Enable static website hosting in the bucket properties.

Upload Files: Use the AWS CLI or Management Console to upload the files:

aws s3 sync ./src s3://your-portfolio-bucket --acl public-read

Set Bucket Policy: Add a bucket policy to make the files publicly accessible (if needed for static website hosting).

Custom Domain Setup (Optional):

Configure your domain in Route 53.
Use AWS Certificate Manager to enable HTTPS.

CloudFront Integration (Optional):

Set up a CloudFront distribution for caching and HTTPS support.

Access the Website
Visit the website URL provided by the S3 bucket or CloudFront distribution.

Portfolio-aws-s3/
├── src/
│   ├── index.html         # Main HTML file
│   ├── styles/            # CSS files
│   ├── scripts/           # JavaScript files
│   └── assets/            # Images and other media
├── README.md              # Project documentation

Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue to suggest improvements.

License
This project is licensed under the MIT License. You are free to use, modify, and distribute this code as per the license terms.

Contact
For questions or suggestions, feel free to reach out:

Email: devjkhuman17@gmail.com
Portfolio: http://tws-dev-portfolio-devops.s3-website-us-east-1.amazonaws.com/




