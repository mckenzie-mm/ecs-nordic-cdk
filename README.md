# CDK 

Demonstration setup for the company 'Nordicmade' based in Norway (https://www.nordicmade.com/) 

This is the CDK code for the deployment to an AWS Elastic Container Service (ECS) of the Nextjs frondend code and the dotnet backend API code  as a mircoservice.

The ECS runs both the Nextjs and dotnet apps (docker containers) on the same task using an EC2 cluster.

The task uses a bridge network for communicating between the containers.

The `cdk.json` file instructs the CDK Toolkit how to execute the app.

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `npx cdk deploy`  deploy this stack to your default AWS account/region
* `npx cdk diff`    compare deployed stack with current state
* `npx cdk synth`   emits the synthesized CloudFormation template
# ecs-nordic-cdk

Inline-style: 
![alt text][https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/1.png](https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/1.png)
