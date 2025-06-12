# CDK 

This is the CDK part of the demonstration setup for the company 'Nordicmade' based in Norway (https://www.nordicmade.com/) 

The code is a Nextjs/dotnet replacement for the "savoy" Wordpress app built by Nordicmade:

http://3.26.70.15/

The CDK code deploys the app as a microservice to an AWS Elastic Container Service (ECS) with the Nextjs frondend code and the dotnet backend API code.

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

![alt text](https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/1.png)

![alt text](https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/2.png)
