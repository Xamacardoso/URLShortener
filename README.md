# URLShortener
A URL Shortener project using Java, AWS Lambda, AWS S3 and other technologies

# About this Project
This project consists in a URL shortener using AWS as a serverless infrastructure.
It allows users to create short URLs that redirect to the original URLs, with
an adjustable expiration time. The system is composed mainly by two lambda functions.
The first one **generates and stores** shortened links in a S3 Bucket, also storing informations like
the original URL and the expiration time. The second one **manages redirecting**, verifying the short URL code
and validating if the generated URL is still within expiration time before redirecting the user.
