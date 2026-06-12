flowchart TD
    User --> CloudFront
    CloudFront --> S3[Static Website - S3]
    CloudFront --> APIGW[API Gateway]
    APIGW --> Lambda[AWS Lambda]
    Lambda --> DynamoDB["(DynamoDB)"]
