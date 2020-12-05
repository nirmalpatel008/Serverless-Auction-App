# Serverless-Auction-App
Serverless Auction App is built to have hands-on experience of Serverless Framework and different AWS services like DynamoDB, lambda, API Gateway, S3, SQS, EventBridge, and SES.

# AWS Services used
* Amazon DynamoDB (Auction Data Persistence)
* AWS Lambda (For CRUD Functionality & Authentication)
* Amazon S3 (Upload an Auction Picture)
* Amazon API Gateway (For HTTP APIs & Authorizer)
* AWS EventBridge (Periodically closing Auction After 1 hour)
* Amazon SQS (To send messages between microservices using queue)
* Amazon SES (To send notification via email for seller and bidder)

# Deployment
## Prerequisite
1) Install Nodejs and NPM. [Click here to install Node.Js](https://nodejs.org/en/download/")
2) Install AWS CLI. [Click here to install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html")
3) Install Serverless Framework. [Click here to install Serverless Framework](https://www.serverless.com/framework/docs/providers/aws/guide/installation/")
4) Configure AWS CLI with Profile. [Click here to configure AWS CLI with Profile.](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html")

## Deploy the Microservices
1) clone this repository.
   ```
    https://github.com/nirmalpatel008/Serverless-Auction-App.git
    ```
2) Move into this path.
   ```
   cd Serverless-Auction-App/Back-End Microservices/
   ```
3) Install the packages inside each microservices
    ```
    npm install
    ```
4) Deploy each microservice using this command. 
  (path must be like this ```cd/Serverless-Auction-App/Back-End Microservices/auction-service```)
   ###### Deploy microservice in this order notificication-service , auth-service, auction-service. 
    ```
    sls deploy -v
    ```
5) Removing the Stack
    ```
    sls remove -v  
    ```
  
  
