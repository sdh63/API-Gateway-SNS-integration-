# API-Gateway-SNS-integration-
In this project you will learn how to use API Gateway within AWS, together with Mock, Lambda and Direct AWS Service Integrations. This will give you experience of all these services as well as how to implement simple, serverless event driven back-end architectures
Please read the instructions below.
I can certainly help you create a step-by-step document based on the video content. Here's a structured guide following the instructions provided in the video:

**Creating an API with AWS Gateway and Lambda:**

1. **Log into AWS Account** [00:00:29][^1^][1]
   - Ensure you have admin permissions.
   - Use the Northern Virginia region (US-East-1) for this project.

2. **Create SNS Topic** [00:01:16][^2^][2]
   - Navigate to SNS console, create a new topic named "API-Messages."
   - Set publishers and subscribers to your AWS account.

3. **Set Up Email Subscriber** [00:02:36][^3^][3]
   - Under the created topic, add a new subscription using your email.
   - Confirm the subscription via the received email.

4. **Create Lambda Function** [00:03:34][^4^][4]
   - Open Lambda console, create a function named "api-return-ip" using Python 3.9.
   - Delete the placeholder code and deploy the provided code snippet.

5. **Create API in API Gateway** [00:04:45][^5^][5]
   - Open API Gateway console, create a new Rest API named "My-Demo-API."
   - Ensure it's a regional API.

6. **Create Mock Resource** [00:05:54][^6^][6]
   - Add a new resource named "Mock" for testing purposes.
   - Configure the mock integration to return a custom JSON message.

7. **Create Lambda Resource** [00:08:20][^7^][7]
   - Add a new resource named "Lambda" to integrate with the Lambda function.
   - Set up the Get method to invoke the Lambda function and return data.

8. **Set Up AWS Service Integration** [00:10:15][^8^][8]
   - Create a role in IAM for API Gateway to publish messages to SNS.
   - Add a new resource named "SNS" in API Gateway.
   - Configure the Post method to integrate with SNS using the created IAM role.

9. **Deploy API** [00:16:20][^9^][9]
   - Deploy the API to a new stage named "V1."
   - Test each integration by accessing the invoke URL with the appropriate resource path.

10. **Clean Up AWS Resources** [00:21:43][^10^][10]
    - Delete the created API, SNS topic, subscriptions, Lambda function, and IAM roles.
    - Ensure the account is back to its initial state.

Remember to replace placeholders with your specific details, such as the AWS account ID and email address. Also, make sure to follow the security best practices when handling AWS resources.
