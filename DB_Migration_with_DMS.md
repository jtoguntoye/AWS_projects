- In this advanced demo you will be migrating a simple web application (wordpress) from an on-premises environment into AWS.
- You will be migrating this into AWS and running the architecture on an EC2 webserver and RDS managed SQL database.

### Architecture

![LucidChart_DMS_DB_MIGRATION](https://user-images.githubusercontent.com/23315232/177317640-a753fb41-2f9d-44e7-8db5-f3ae185bcddd.png)

- STAGE 1 : Provision the environment and review tasks
- STAGE 2 : Establish Private Connectivity Between the environments (simulateed using VPC Peer in this demo)
- STAGE 3 : Create & Configure the AWS Side infrastructure (App and DB)
- STAGE 4 : Migrate Database & Cutover


### DMS Creation stack

[AWSTemplateFormatVersion.pdf](https://github.com/jtoguntoye/AWS_projects/files/9046036/AWSTemplateFormatVersion.pdf)

### Stage 1
Click https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/quickcreate?templateURL=https://learn-cantrill-labs.s3.amazonaws.com/aws-dms-database-migration/DMS.yaml&stackName=DMS to apply the base lab infrastructure

You should take note of the parameter values

- DBName
- DBPassword
- DBRootPassword
- DBUser

You will need all of these in later stages.
All defaults should be pre-populated, you just need to scroll to the bottom, check the capabilities box and click Create Stack
