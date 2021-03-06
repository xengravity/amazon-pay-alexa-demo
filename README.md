# Amazon Pay for Alexa Demo
This is a 'bare-bones' demo to show how you can integrate Amazon Pay into your Alexa skill.  

## Getting Started
Read the integration guide: https://developer.amazon.com/docs/amazon-pay/amazon-pay-overview.html
  
Once your [Alexa](https://alexa.amazon.com/), [Amazon Pay](https://pay.amazon.com/), [AWS](https://aws.amazon.com/), and [Developer](https://developer.amazon.com/) accounts are ready you can modify this skill.
1. Clone repository and install dependencies
2. Open [config.js](config.js) and update values `appID`, `sellerId`, and `sandboxCustomerEmailId`
3. [Zip files and upload to Lambda](https://developer.amazon.com/docs/custom-skills/deploy-a-sample-skill-to-aws-lambda.html#preparing-a-nodejs-sample-to-deploy-in-lambda)
4. [Link your accounts](https://developer.amazon.com/docs/amazon-pay/integrate-skill-with-amazon-pay-v2.html#link_sc)
5. [Enable testing](https://developer.amazon.com/docs/devconsole/test-your-skill.html) for your skill and invoke it:  

  ![alt text](https://i.imgur.com/joMdlZl.png)

If you receive the message `Thank you for ordering form Blitz and Chips` then you have successfully configured your skill! If you receive an error, proceed to the [troubleshooting section](https://github.com/xengravity/amazon-pay-alexa-demo#troubleshooting).

## Troubleshooting

If you are encountering issues with your skill, double check that you have completed the following:

1. Confirm that your Seller Central account is in good standing by selecting the Production environment and verify there are no errors on your account
2. Link the correct skill in the appropriate environment ( Sandbox / Production ) in Seller Central
3. Create a sandbox buyer test account in Seller Central
4. Enable Amazon Pay permissions in your skill under Build > Permissions > Amazon Pay
5. Link the correct Lambda function in your skill under Build > Endpoints > Default Region
6. Upload the correct .zip file with the updated values in config.js
7. Link the correct skill Id in your Lambda function
8. Give the correct permissions for the role to use your Lambda function
9. Enable your skill in your Alexa App
10. Consent and give permissions to Amazon Pay in your Alexa App
11. Enable Voice Purchasing in your Alexa App

All other errors and decline handling can be found here: https://developer.amazon.com/docs/amazon-pay/payment-declines-and-processing-errors.html
