# Project2 deploy-a-high-availability-web-app-using-CloudFormation


> In this project (Udagram App), I deployed web servers for a highly available web app using CloudFormation.
> I have created the script that deploys the infrastructure and Servers used for The Udagram app.

## Project Files:
```sh
1- create.sh : Cloudformation create stack script. 
2- update.sh : Cloudformation update stack script.
3- ourinfraServer.yml : Udagram Project's CloudFormation script.
4- ourinfraServerParameters.json : Udagram Project's CloudFormation script parameters.
```
## Instruction of deploy:
Just run;
```sh
> ./create.sh UdagramApp infrastructure.yml infrastructure.json
```aws cloudformation create-stack --stack-name udagramApp --template-body file://ourinfraServer.yml --parameters file://ourinfraServerParameters.json --capabilities CAPABILITY_NAMED_IAM

aws cloudformation update-stack --stack-name udagramApp --template-body file://ourinfraServer.yml --parameters file://ourinfraServerParameters.json --capabilities CAPABILITY_NAMED_IAM
