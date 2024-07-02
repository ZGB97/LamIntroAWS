<h1> Automated EC2 Instance Management with AWS Lambda (AWS) </h1>


<h2>Description</h2>
In this lab, I created an AWS Lambda function and set up an Amazon EventBridge event to trigger the function every minute. The Lambda function, using an IAM role, stops a running EC2 instance in my AWS account. First, I accessed the AWS Management Console and launched the lab environment. Then, I created a Lambda function named myStopinator with Python 3.8 as the runtime and assigned it an existing IAM role. Next, I configured an EventBridge rule to trigger the function every minute. I updated the Lambda function's code to stop a specific EC2 instance by replacing placeholders with my region and instance ID. Finally, I deployed the code and verified that the Lambda function successfully stopped the EC2 instance by checking the instance status in the EC2 console.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Amazon Web Services (AWS) Management Console: For setting up the Lambda function and EventBridge rule.</b>
- <b>AWS Lambda: For running the serverless function.</b>
- <b>Amazon EventBridge: For scheduling the function trigger.</b>
- <b>AWS Identity and Access Management (IAM): For managing access permissions.</b>
- <b>Python: As the runtime for the Lambda function.</b>
- <b>boto3: AWS SDK for Python, used in the Lambda function to interact with EC2.</b>

<h2>Program Screenshots:</h2>

<p align="center">
Lambda function configuration: <br/>
<img src="https://i.imgur.com/HxKIbKT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Scheduled event configuration:  <br/>
<img src="https://i.imgur.com/9WzmPvc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Updated Lambda function code including actual Instance ID: <br/>
<img src="https://i.imgur.com/9eqnGsl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Verify that the Lambda function worked:  <br/>
<img src="https://i.imgur.com/DwlRNnx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
