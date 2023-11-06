# AWS Hello World

*A simple project to get an AWS web app in production. Using AWS CLI whenever possible for deployment.*

- **Frontend**: React app hosted on S3
- **Backend**: Serverless API with Lambda and API Gateway


## Next Potential Steps When Done:
1.  TypeScript-ify the React app → is that a verb? ...write it in TypeScript!
2.  AWS Aurora Serverless → set up a super simple database and write an API function to get / write data

## Steps:
### 1. Local Development Environment Setup:
* Install Node.js and npm on your local machine.
* Install and configure AWS CLI with the necessary permissions.
### 2. Initialize Your React Project:
* Create a new React app locally using create-react-app.
* Develop your React application and implement the frontend logic.
* Implement a function to call the backend API when needed.
### 3. Prepare the Backend API:
* Write a simple Lambda function in your chosen language that returns the desired response.
* Configure AWS API Gateway to create a new API endpoint that triggers the Lambda function.
* Test the API endpoint using a tool like Postman or AWS Console to ensure it’s returning the correct response.
### 4. Integrate the API with Frontend:
* Update your React app to call the API Gateway endpoint and process the response.
* Test the integration locally to ensure the React app behaves as expected when calling the backend API.
### 5. Build the React Application:
* Run the build script to compile your application into static files.
### 6. Create an S3 Bucket for Hosting:
* Use AWS CLI to create a new S3 bucket.
* Configure the bucket for static website hosting.
### 7. Deploy the React App to S3:
* Upload the build artifacts to the S3 bucket using AWS CLI.
* Update the bucket policy to allow public read access to the website files.
### 8. Set Up Domain and SSL (Optional):
* Register a domain name with Route 53 or another domain registrar if you don’t already have one.
* Create a CloudFront distribution to serve your S3 content over HTTPS.
* Associate your domain with the CloudFront distribution.
### 9. Configure CORS for API Gateway:
* Modify CORS settings on API Gateway to allow your S3 hosted domain to call the backend API.
### 10. Test the Application in Production:
* Access the React app via the S3 website URL or custom domain.
* Verify that the frontend can successfully call the backend API and update the content on the screen.
### 11. Monitor and Troubleshoot:
* Set up CloudWatch logs for your Lambda function to monitor its usage and errors.
* Optionally, enable additional logging or monitoring through AWS services for your S3 hosted content and API Gateway calls.
### 12. Iterate and Update:
* For future updates, repeat the build and deploy steps (5, 7) for your React app.
* Update the backend Lambda function and API Gateway configuration as needed.
