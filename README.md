# Robo Advisor
This project uses Amazon Web Services (AWS) to create a bot that customers can use to get investment portfolio recommendations for retirement. The prototype bot project is divided into three steps:
1. Configure the initial robo advisor
2. Build and test the robo advisor
3. Enhance the robo advisor with an Amazon Lambda function


## Technologies from AWS Management Console:
* [Amazon Lex](https://docs.aws.amazon.com/lex/latest/dg/what-is.html) - an AWS service for building conversational interfaces for applications using voice and text that enables you to build sophisticated, natural language chatbots into new and existing applications. 
* [Amazon Lambda](https://docs.aws.amazon.com/lambda/?id=docs_gateway): a compute service that lets you run code without provisioning or managing services on a high-availability compute infrastructure and performs all of the administrations of the compute resources. 


## Installation Guide
Click on the link below and complete the following task:
1. [Sign up for AWS](https://docs.aws.amazon.com/lex/latest/dg/gs-account.html#gs-account-create) 
2. Create an IAM User
3. Get Started in Console
4. Use the search bar to look up Amazon Lex service
5. Use the search bar to look up AWS Lambda


## Usage and Features
### **Configure the initial robo advisor**
Amazon Lex bot with the following criteria:
   * Bot name: RoboAdvisor
   * Language: English (US)
   * Output voice: Salli
   * Session timeout: 5 minutes
   * Sentiment analysis: No
   * COPPA: No
   * Advance options: No
   * All other options: The default value

Add a new intent, named `recommendPortfolio`

Configure sample utterances (Typed phrases that invoke your intent):

<img width="446" alt="image" src="https://user-images.githubusercontent.com/96001018/163515730-52d78c7c-e45b-4989-bc71-5d5f19747e8c.png">

Slots (Data the user must provide to fulfill the intent):

<img width="614" alt="image" src="https://user-images.githubusercontent.com/96001018/163515787-56d88d82-20f3-469c-a3ab-167dded48646.png">

Confirmation Prompt (Questions that ask the user to input data):

<img width="617" alt="image" src="https://user-images.githubusercontent.com/96001018/163516177-d97f1cf3-ed76-46e3-b999-8366b18ef34f.png">

### **Build and test the robo advisor**

Test bot showing a simple test conversation:

![test_bot1](https://user-images.githubusercontent.com/96001018/163523884-e3ca2249-aa8d-45f3-a3b0-6d97ebd71a4d.gif)


### **Enhance the robo advisor with an Amazon Lambda function**

Enhance the robo advisory by using the Lambda function. Code is included in this repository in the `Lambda` folder, select `lambda_function.py`. This function contains code that validates rules of `age` values are greater than zero and less than 65. Also validates `investment_amount` value should be greater than or equal to 5000. The bot will respond with an investment recommendation based on the selected risk level. 

The Lambda function is integrated into the bot: 

<img width="283" alt="image" src="https://user-images.githubusercontent.com/96001018/163516852-3105dc0d-78f8-4286-85fc-48be3464d4d6.png">

<img width="353" alt="image" src="https://user-images.githubusercontent.com/96001018/163516904-4d0b9158-ed7a-42e0-a207-0ccd1abd1f6d.png">


Enhanced robo advisor with Lambda function:

![robo_bot](https://user-images.githubusercontent.com/96001018/163526506-83d282bd-156e-464e-b04b-db715d044bf6.gif)

## Contributors

Leigh Anne Badua leighbadua@gmail.com 


## License

Creative Commons Zero v1.0 Universal 
