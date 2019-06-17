# SESEmailForward
Amazon SES Email Forward to Your Inbox

![picture](SESEmail.png)

[![Deploy Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=SESEmailForward&templateURL=https://s3-us-west-2.amazonaws.com/alikian.me/forwarder.yaml)

## Usage Guide
You can deploy the CloudFormation stack which will provision the following AWS Services
- SNS Topic to forward, received emails from SES
- RuleSet and Rule to forward Recipient to SNS topic
- IAM Role to invoke Lambda function from SNS
- Lambda function with NodeJS code to forward the emails to a defined from and to address
- IAM Role allowing Lambda to forward emails.

You need to active RuleSet in SES

## Tips
- Make sure sender and forwarder emails are verified in SES
- Make sure Recipient email or domain is verified
