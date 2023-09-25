         ___        ______     ____ _                 _  ___  
        / \ \      / / ___|   / ___| | ___  _   _  __| |/ _ \ 
       / _ \ \ /\ / /\___ \  | |   | |/ _ \| | | |/ _` | (_) |
      / ___ \ V  V /  ___) | | |___| | (_) | |_| | (_| |\__, |
     /_/   \_\_/\_/  |____/   \____|_|\___/ \__,_|\__,_|  /_/ 
 ----------------------------------------------------------------- 


Hi there! Welcome to AWS Cloud9!

To get started, create some files, play with the terminal,
or visit https://docs.aws.amazon.com/console/cloud9/ for our documentation.

Happy coding!
Analysis: The CloudFormation template that ran when you started this lab created resources in the AWS account. The script you ran also created resources. Between the two of them, the following resources have been created to replicate what you built in previous labs:
An S3 bucket with an associated bucket policy. The bucket contains the café website code.
An Amazon DynamoDB table populated with menu data.
A REST API configured using Amazon API Gateway.
An AWS Lambda function that retrieves data from DynamoDB when invoked.
A Memcached cluster that caches supplier data from Amazon Aurora Serverless for the suppliers application. A café/node-web-app Docker image, which is stored in the Amazon Elastic Container Registry (Amazon ECR).
An AWS Elastic Beanstalk environment and application that runs an EC2 instance named MyEnv. The EC2 instance hosts a Docker container created from the Docker image that is stored in Amazon ECR.
An Aurora Serverless database running MySQL on Amazon RDS, which contains the supplierdb database, which stores coffee supplier information.

![template1-designer (3)](https://github.com/jipx/pythonnodejs-lab-9.2/assets/4178277/1de36d62-0d15-430d-9f6c-a24620e7ae9c)
