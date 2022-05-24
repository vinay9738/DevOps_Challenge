Logical layers in Three-tier Architecture:
The Three-tier architecture consists of three logical layers:
i) presentation layer
ii) bussiness layer
iii) data storage layer.

My approach to this Architecture:

This diagram shows a brief Explanation on how the 3-Tier Architecture has been designed,and what all Cloud Products and services are used to Deploy the applications 
using Jenkins CI/CD Pipelines in Kubernetes Rancher Clusters. The Cloud Architecture for applications has a bias towards Iaas based services. In this diagram I have used the backup necessary for the project to avoid any accidental loss of data. One VPC is created each for Dev, Stage, production and management with the same architecture set up and is been connected using VPC peering. I have added route 53 which is used to route the end users to internet applications which translates the web names into the numeric form. AWS Direct connect is used in this architecture to connect from the on-premises which is then conncted to the VPC by a central hub called transit gateway. Load balancer will help to distribute the incomming application traffic signals across the worker nodes. I have used Rancher here which can help me in managing multiple kubernetes clusters. The applications are stored in Nexus 3 repository in form of a Container image and is deployed to kubernetes clusters which is managed by the Rancher.

The Key AWS cloud services used in solution are:

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

Jenkins CI/CD Pipelines process is explained in the seperate file.
