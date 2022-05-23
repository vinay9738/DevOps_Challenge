Brief Explanation on how the 3-Tier Architecture has been designed,and what all Cloud Products and services used to Deploy applications 
using Jenkins CI/CD Pipelines in Kubernetes Rancher Clusters. 

The Cloud Architecture for applications has a bias towards Iaas based services. Ke AWS cloud services used in solution are:

Storage - EBS, S3
Networking - VPC, VPC Peering, Route 53, AWS Direct Connect, Load Balancers, Transit Gateway
Compute - EC2, ECR
DNS - Route 53
Security, Identity and Compliance - Guard duty, IAM, Secret Manager, Certificate manager
Development - CloudFormation(IAC)
Cost Management - Cost and usage reports

Application Components - Rancher 2x, Kubernetes, Web Based Java applicatons

Compute Infrastructure :

Cluster and app managemet - Rancher
Containerisation Platform - Docker
Container orchestration Kubernetes (Deploed as Rancher as RKE)
Oracle DB host operating system - Redhat

Jenkins CI/CD Pipelines process as in attached doc
