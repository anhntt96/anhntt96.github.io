### Domain 1: SDLC Automation 22%
- Focus on SDLC and AWS developer tools
- Take time to build and using CodePipeline:
  - Understand each stage and the option of each stage
  - Dive deeper into the deployment stage:
    - AWS CloudFormation
    - AWS CodeDeploy
  
### Domain 2: Configuration Management and IaC 17%
- Focus on composing and deploying template
- need depth with 
  - CodeDeploy
  - CloudFormation: also know the helper script and their use cases
  - Opswork
  - Elastic Beanstalk
- Open questions:
  - What these service do?
  - Their use cases?
  - When to use each one over another?
  - Deployment and deployment methods you use?

### Domain 3: Resilient Cloud Solutions
- Focus on:
  - building and managing highly available, scalable, and reliable systems using multiple availability zones and services, such as auto scaling and load balancing
  - Multi region services such as DynamoDB Global Tables
  - Disaster recovery and understanding how to determine and monitor requirements for recovery time objective (RTO) and recovery point objective (RPO)
  - How much data back is needed 

### Domain 4: Monitoring and Logging 15%
- Service focus:
  - Amazon CloudWatch
  - Amazon EventBridge
  - Amazon Kinesis family (real-time)

### Domain 5: Incident and Event Response 14%
- Adding automation to ensure your systems are reliable.
- How to use the correct metrics to ensure that reliability.
- Service focus:
  - AWS Systems Manager
  - Kinesis
  - AWS Simple Notification Service
  - AWS Lambda
  - CloudWatch (especially alarms)
  - Amazon EventBridge
  - How to receive on-premises server log(CloudWatch logs agent)
  - How to manage those on-prem servers (AWS Systems Manager Agent)

### Domain 6: Security and Compliance 17%
- How to manage identity and access management at scale, apply automation for data protection and security controls.
- Implement security monitoring
- Service focus:
  - IAM
  - AWS Security Hub
  - AWS WAF
  - VPC Flow logs
  - AWS Certificate Manager
  - AWS Config (Audit and auditing)
  - Amazon Inspector
  - Amazon GuardDuty
  - Amazon Macie
  - AWS Trust Advisor
  - AWS System Manager (when to use each service/feature)

### Helpful links

- [tutorialsdojo DOP-C02 eaxm guide](https://tutorialsdojo.com/aws-certified-devops-engineer-professional-exam-guide-study-path-dop-c01-dop-c02/) 


### Labs

#### AWS Lambda
- [Building Lambda functions with Node.js](https://docs.aws.amazon.com/lambda/latest/dg/lambda-nodejs.html)
  - includes [Sample Lambda applications](https://github.com/awsdocs/aws-lambda-developer-guide/tree/main)
- [Tutorial: Building a serverless chat app with a WebSocket API, Lambda and DynamoDB](https://docs.aws.amazon.com/apigateway/latest/developerguide/websocket-api-chat-app.html)
- [Tutorial: Building a serverless application with three integration types](https://docs.aws.amazon.com/apigateway/latest/developerguide/websocket-api-step-functions-tutorial.html)


#### AWS CloudFormation
-  [Creates a WordPress blog as a stack](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/GettingStarted.Walkthrough.html)



Amazon EventBridge
Amazon CloudWatch Alarms
AWS CodePipeline
AWS CodeDeploy
AWS CodeBuild
AWS CodeCommit
AWS Config
AWS Systems Manager
Amazon ECS
Amazon Elastic Beanstalk
AWS CloudTrail
AWS OpsWorks
AWS Trusted Advisor