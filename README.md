# CDK 

This is the infra-structure as code (AWS CDK) part of the demonstration website built for the company 'Nordicmade' based in Norway (https://www.nordicmade.com/) 

The code is a Nextjs/dotnet replacement for the "savoy" Wordpress app built by Nordicmade. The demonstration website is at: http://3.26.70.15/

The CDK deploys the app as a microservice to an AWS Elastic Container Service (ECS) with the Nextjs frondend code and the dotnet backend API code.
The front end codeis at https://github.com/mckenzie-mm/nordic-frontend. The dotnet backend is at: https://github.com/mckenzie-mm/nordic-api

The app runs on an AWS container service (ECS). This was chosen instead of Kubernetes due to the lower cost and ease with which a demonstration setup could be configured with ECS. It is currently deployed only on the Australian AWS region and will be slow to load in Europe/Norway. 

The ECS runs both the Nextjs and dotnet apps (docker containers) on the same task using an EC2 cluster.

The task uses a bridge network for communicating between the containers.

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `npx cdk deploy`  deploy this stack to your default AWS account/region
* `npx cdk diff`    compare deployed stack with current state
* `npx cdk synth`   emits the synthesized CloudFormation template
# ecs-nordic-cdk

The main part of the infrastructure is shown in the code extract below. It is currently deployed only on Australian AWS and will be slow to load in Europe/Norway.

![alt text](https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/1.png)
![alt text](https://github.com/mckenzie-mm/ecs-nordic-cdk/blob/main/images-readme/2.png)
