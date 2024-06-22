# Questions

## Management
- Intro/tell me about yourself
  - from surat
  - completed graduation in 2021 
  - with 2.5+ years of experience in creating, configuring, and managing ci/cd pipelines and cloud resource 
- why do you want to leave
- Let's say you have been given a task and that task's deadline is 7 days, but client forgot to assign access to perform the task it took 3 days to assign access and then you can start working on a task, how you will handle this situation, what are the steps you will take
- let's say I have given you a task to create infrastructure for an application, what are the questions you will ask me regarding the task?
- 


## Kubernetes:
- what is Kubernetes and why 
- what is disadvantage of Kubernetes 
- prepare architecture 
- replicasets and replication controller 
- pod and deployment 
- statefulsets and deployment 
- what is the ingress, why ingress 
- what is cluster-issuer 
- pvc and pv
  - pvc autoscaler 
  - what are different accessmode in PVC
	- ReadWriteOnce, ReadWriteMany, ReadOnlyMany, ReadWriteOncePod
	- difference between ReadWriteOncePod and ReadWriteOnce
  - what are different reclain policies pvc
    - Retain, Delete, Recycle
  - what are the differnt Phase of pv
    - Available, Bound, Released, Failed
- what is storage class 
- what is kube proxy 
- what does API server 
- static pods 
  - schedule a pod on specific node without scheduler 
- RBAC 
- hpa, vpa
- keda 
- taint toleration
- pod and node affinity 
- node selectors 
- metal lb 
- default port of k8s 
- network policy in Kubernetes 
  - ingress and egress 
  - 
- shield secrets 
- request limit 
- types of services 
- current version: 1.29
- latest version: 1.30


## Terraform
- terraform init
- terraform backend, remote backend 
- secret management in terraform 
- terraform modules 
- how to use vpc module in ec2 module 
- write a sample terraform file to print Hello World 
- what are providers 
- what are provisioners 
- what is the disadvantage of terraform 
- API as code 
- use case of null resource 
- what are different data types in terraform 
- difference between for each and count 
- how to create multi-region aws resource 
  - provider region alias 
- terraform best practices 
- parallelism in terraform 
  - default is 10 
  - terraform apply -parallelism=20
  - Configuring terraform.rc (or .terraformrc) default parallesim
- current terraform version: 1.6 
- latest version: 1.8.5



## AWS Services 
- Ec2
  - default storage disk 
  - can we increase 
- VPC
  - peering
  - multi-account access 
- subnets
  - privet and public subnets 
- IAM
  - difference role, policy, user
- Security groups
- Autoscaling groups
  - launch templet 
  - 
- route table 
  - subnet association 
- internet gateway 
- net gateway 
- vpn
- direct connect
- Load Balancers ( types )
  - 4 types ( Application, Network, 
- EKS 
  - storage classes ( default gp2 ebs type )
    - dose default storage class has policies like 
  - eksctl
  - which iam roles are required to run eks cluster 
  - Default network plugin in eks is "VPC CNI"
  - what are differnet options of network plugin for eks 
- Lemda ( max run time 15 min ) 
- different storage services 
  - ebs, efs, 
- s3 
  - policy 
  - CLI 
  - types 
    - standard, infrequent access, glacier, glacier deep archive, intelligent type
  - if I put an object in 1 bucket then it should clone to another bucket
- route 53 
  - hosted zone 
- what are launch templets in aws ( eks, ecs )
- what is a disadvantage of cloud computing 
- What is the advantage of cloud computing 
- ECS
  - cluster 
  - task definition 
- how to connect eks with s3 
- eksctl 
- how to decide database service 
  - different types of database services 
- how to configure waf 
- i have configured ec2 with rds but it is not working list the potential issues 
- elastic IP 

## Azure Services 
- AKS
  - what are differnet options of network plugin for 
  - default network plugin 
- ACR
- VMSS
- Front Door 
- CDN
- Cosmodb (multi-region write configuration ) 
- Traffic Manager 
  - health check 
  - priority
  - weight
  - endpoint 
- Blob containers 
- Azure fileshare
- Azure DNS zone ( 1500 records )
- Azure Communication service 
- IAM
  - how to assign access on whole tenant 
- different types of database services 
- WAF 


## Git GitHub
- what is pull request 
- git pull and fetch 
- git clone 
- git rebase and merge 
- 


## Docker
- docker add vs copy 
- docker entrypoint and cmd 
- Multi-stage docker image 
- what is docker 
- build arguments in docker 
- what is default path of docker 
- how to change default path of docker 
- different types of networks 
- different types of storage drivers 


## CICD 
- Jenkins
  - what is declarative pipeline 
  - how to add agents in Jenkins 
- Azure Devops
  - how to add agents in Azure DevOps 
  - deployment groups in azure devops 
  - azure artifacts 
- ArgoCD 
  - you have to create an app where provide URL/path of the manifest 


## Shell Scripting Linux 
- sed command 
- what is fstab 
- what is bashrc 
- basic monitoring commands 
- Types of DNS Records
  - A, CNAME, MX, PTR
- what is TCP, UDP difference
- OSI model
- special permissions: sticky bit
- what is umask
- what is daemon, difference daemon and process 
- grep command 
  - -v for exclude
  - multiple in grep 

## Ansible
- what is default path for hosts 
- how to check host is accessible or not 
- ansible facts 
- 


## Prometheus, Grafana, loki, elk stack 
- promql 
- elk configuration, efk configuration 
- created custom dashboards 
- 

## Other tools 
- airflow, statsd exporter 
- Kafka 
- chatwoot
- casdoor
- keycloak
- vaultwarden
- crunchydb
- trino
- ETL pipelines
- mailserver, mailcow, mailcow exporter 
- TSDB
- rocket chat
- pgadmin 
- pgbouncer
- allure reports, cucumber testing 
