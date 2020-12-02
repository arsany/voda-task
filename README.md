# Voda-Task

 

## In This Project

  -  Working in AWS
  - Using Jenkins to implement Continuous Integration and Continuous Deployment
  -  Building pipelines
  -  Working with CloudFormation to deploy clusters
  -  Building Kubernetes clusters
  -  Building Docker containers in pipelines



## Steps
- Using CloudFormation IaC deploy (EKS Cluster and Jenkins-machine) from infrastructure dir

```bash
aws cloudformation create-stack --stack-name voda-task --template-body file://amazon-eks.yaml --capabilities CAPABILITY_NAMED_IAM 
aws cloudformation create-stack --stack-name jenkins-machine --template-body file://jenkins-machine.yaml --capabilities CAPABILITY_NAMED_IAM
```
- After CF complete you can configure Jenkins from console and don't forget to add credentials for 
 

 ```bash
 Docker "docker_hub_login"
 sshagent "Project"
 ```


[Enjoy](https://www.linkedin.com/in/arsanyatya92/)
