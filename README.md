# survey-report-generator
POC Project for generating report for GPS survey project. Will leverage AWS Serverless architecture  

### Components
- Webapplication - SPA (s3 + cloudfront + route53) -> s3
    - React application
    - Upload file to s3 bucket
    - call webpi to trigger data processing
    - display the output to end users
- S3 buckets 
    - to store objects uploaded by user
    - to store output report
    - to store react website
- Lambda Job (python lambda job) 
    - reads the S3 file
    - generates the results
    - writes the report back to s3
- Webapi (python lambda job + api gateway + route53)
    - tigger lambda job
    - getch the progress
    - get lambda job results

### Automation
    - Cloud formation template
    - CI/CD pipeline using Codebuild
### Steps
    - [] Create S3 Buckets
    - [] Create React application and Deploy it
    - [] Create Web api - python
    - [] Create python lambda job for data processing


