# AWS-Lambda-CRUD-Sample
AWS Lambda CRUD Sample


#First Step
Log in in your AWS account

#Second Step
Create a Table in DynamoDB (in my case, for purpose of this demo: products)

#Create a Lambda Function
Select:
  - Author from scratch
  - Define a function Name
  - Select Node runtime (for the purpose of this demo)
  - Select: "change default execution role"
    - Select: "Create a new role from AWS policy templates"
    - Enter a role name
    - Select the following role: "Simple Microservice Permission" (and add it)
  - Select "Create Function"

#In the Lambda Function
Paste the Lambda.js code in "index.js" file
Click "Deploy"

#In API Gateway
  - Create API
  - Select HTTP 
