# Amazon Pay for Alexa Demo
This is a 'bare-bones' demo to show how you can integrate Amazon Pay into your Alexa skill.  

## Getting Started
Read the integration guide: https://developer.amazon.com/docs/amazon-pay/amazon-pay-overview.html
  
Once your [Alexa](https://alexa.amazon.com/), [Amazon Pay](https://pay.amazon.com/), [AWS](https://aws.amazon.com/), and [Developer](https://developer.amazon.com/) accounts are ready you can modify this skill.
1. Clone repository and install dependencies
2. Open [config.js](config.js) and update values `appID`, `sellerId`, and `sandboxCustomerEmailId`
3. [Zip files and upload to Lambda](https://developer.amazon.com/docs/custom-skills/deploy-a-sample-skill-to-aws-lambda.html#preparing-a-nodejs-sample-to-deploy-in-lambda)
4. [Link your accounts together](https://developer.amazon.com/docs/amazon-pay/amazon-pay-overview.html)
5. Enable testing for your skill and invoke it:  
![alt text](https://i.imgur.com/joMdlZl.png)

## Troubleshooting

If you are having issues running the skill, double check the following:
1. Did you link the correct skill in the appropriate environment ( Sandbox / Production ) in Seller Central? 
2. Did you create a sandbox buyer test account in Seller Central?
3. Did you enable Amazon Pay permissions in your skill under Build > Permissions > Amazon Pay
4. Did you link the correct Lambda function in your skill under Build > Endpoints > Default Region
5. Did you upload the correct .zip file with the updated values in config.js?
6. Did you link the correct skill Id in your Lambda function?
7. Did you give the correct permissions for the role to use your Lambda function?
8. Did you enable your skill in your Alexa App?
9. Did you consent and give permissions to Amazon Pay in your Alexa App?
10. Did you enable Voice Purchasing in your Alexa App?

All other errors and decline handling can be found here: https://developer.amazon.com/docs/amazon-pay/payment-declines-and-processing-errors.html
