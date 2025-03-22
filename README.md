# Welcome to your CDK Java project!

This is a blank project for CDK development with Java.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

It is a [Maven](https://maven.apache.org/) based project, so you can open this project with any Maven compatible Java IDE to build and run tests.

## Useful commands

 * `mvn package`     compile and run tests
 * `cdk ls`          list all stacks in the app
 * `cdk synth`       emits the synthesized CloudFormation template
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk docs`        open CDK documentation

```SHELL

$ cdk deploy --all --parameters Rds:databaseUsername=root --parameters Rds:databasePassword=root9876543210 --require-approval never
$ cdk deploy Service01
$ cdk destroy --all

```

Enjoy!

## Reduce AWS costs

### VPC
- Max zones to `2` - maxAzs(2)
- Nat gateways to `0` - natGateways(0)

### Service
- Assign public IP (doesn't have nat) - assignPublicIp(true)