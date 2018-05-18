# Amazon Pay for Alexa Demo
This is a 'bare-bones' demo to show how you can integrate Amazon Pay into your Alexa skill.  
  
Read the integration guide to get started: https://developer.amazon.com/docs/amazon-pay/amazon-pay-overview.html
  
Once your [Amazon Pay](https://pay.amazon.com/), [AWS](https://aws.amazon.com/), [Developer](https://developer.amazon.com/), and [Alexa](https://alexa.amazon.com/) accounts are ready you can use this skill by following the steps below:
1. Clone repository and install dependencies
2. Open [config.js](config.js) and update values `appID`, `sellerId`, and `sandboxCustomerEmailId`
3. Zip files and upload to Lambda

## Troubleshooting

If you are having issues getting the skill to run, double check the following:
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
