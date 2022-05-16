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
  - Select HTTP API
  - Click "Build"
    - Define the API Name
    - N, N, N, Create
  - Now Define the Routes:
    - GET
    - GET {id}
    - DELETE {id}
    - PUT
  - Create the Lambda Integration
    - In integrations, select Managed Integrations, and click in "Create"
    - Select "Lambda Function"
    - Select your Lambda
    - Now in the Attach Integrations to routes, add each route to the same Lambda Function

#Done
Done!
