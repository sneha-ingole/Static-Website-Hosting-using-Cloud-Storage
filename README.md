🌍 Global Launch – Static-Website-Hosting-using-Cloud-Storage


📌 Project Overview

This project demonstrates how to host a personal portfolio website globally using Cloud Storage without provisioning any servers.

The goal was to create a cost-effective, scalable, and globally accessible static website using cloud-native services.

🎯 Scenario

As a freelance developer, the client needed:

-A personal portfolio website

-Global accessibility

-Instant loading worldwide

-No expensive servers

-Low maintenance solution

🚀 Solution

We leveraged Cloud Storage to host a static website.


🔧 Implementation Steps

1.Created a public cloud storage bucket (AWS S3 / Azure Blob Storage)

2.Uploaded static website files (HTML, CSS)

3.Enabled Static Website Hosting

4.Configured bucket policy for public access

5.Generated a public website endpoint URL


🏗️ Architecture

User → Internet → Cloud Storage (S3/Blob) → Static Website Files

No EC2 / No VM / No Server Provisioned.



🛠️ Tools & Services Used

-AWS S3 (Static Website Hosting)

-Bucket Policy (Public Access)

-HTML5

-CSS3

-(Optional) AWS CloudFront for CDN


📂 Project Structure

project-folder/

│

├── index.html

├── style.css

└── assets/

  └── images
    

🔐 Sample Bucket Policy (AWS S3)

{

"Version": "2012-10-17",

  "Statement": [
  
   {
   
    "Sid": "PublicReadGetObject",
    
      "Effect": "Allow",
      
      "Principal": "*",
      
      "Action": "s3:GetObject",
      
      "Resource": "arn:aws:s3:::sneha-ingole/*"
      
      }
      
    ]
    
  }


💡 Key Features

-Serverless hosting

-Highly scalable

-Low cost

-Global accessibility

-Easy deployment

-Secure & reliable


📈 What I Learned

How static website hosting works

-Cloud storage configuration

-Bucket policy management

-Public access control

-Cost optimization in cloud

Global content delivery concepts


🔥 Future Enhancements

Add CloudFront CDN for faster global delivery

Connect custom domain

Enable HTTPS using SSL

Automate deployment using CI/CD



