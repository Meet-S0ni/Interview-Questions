# Questions

## Management
- Intro/tell me about yourself
  - from surat
  - completed graduation in 2021 
  - with 2.5+ years of experience in creating, configuring, and managing ci/cd pipelines and cloud resource 
- why do you want to leave
- Let's say you have been given a task and that task's deadline is 7 days, but client forgot to assign access to perform the task it took 3 days to assign access and then you can start working on a task, how you will handle this situation, what are the steps you will take
- let's say I have given you a task to create infrastructure for an application, what are the questions you will ask me regarding the task?


## Kubernetes:
- what is Kubernetes and why 
- what is disadvantage of Kubernetes 
  - learning curve
  - initial setup
  - security challanges
  - you can not roll back kubernetes version
  - you have to containarized your application
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
- default port of k8s 6443 
- network policy in Kubernetes 
  - ingress and egress 
  - specify 
- shield secrets 
- request limit 
- max surge 
- types of services 
- current version: 1.29
- latest version: 1.30
- what are the majour feature of kubernetes


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
  - there is no error hendaling 
  - we have to use hcl 
  - vender locking, if you have terraform code moving from terraform to another iac is very difficult 
  - state file has sensitive data in plain text
- API as code 
- use case of null resource 
- what are different data types in terraform 
- difference between for-each and count 
- how to create multi-region aws resource 
  - provider region alias 
- terraform best practices 
- parallelism in terraform 
  - default is 10 
  - terraform apply -parallelism=20
  - Configuring terraform.rc (or .terraformrc) default parallesim
- current terraform version: 1.6 
- latest version: 1.8.5
- which components you have created using terraform 
  - resource group, virtual network,subnet,aks cluster, node-pools, acr, kubernetes manifests deployment, helm
  - authanticated using service principle ( app registration )
  - using azurerm, kubernetes, helm,
- terraform command to store output 
  - terraform plan -out file.plan
  - terraform plan --no-colour > file.plan
- what is syntext of terraform import command 
- HCL full form 
  - Hashicorp configuration language 
- what are the majour features of terraform  
  - terraform can manage infrastructure on multiple cloud platforms 
  - terraform uses a language called hcl which is human readable configuration language that helps you to write infrastructure code quickly 
  - terraform also manages after deployment and help to maintain states 
  - we can also version control our code to safely collabrate on our infrasture 
- what is terraform validate command 
  - this command used to validate the syntext of the terraform file, it will check all files in directory and display error if any issue found, it will not check formatting like tabs and spaces 
  - if provider or module declered multiple times than it checks like this 
- how to write comment in terraform 
  - using #  
- can you tell me what is lifecycle in terraform 
  - Terraform, the lifecycle block is used within a resource to define special behaviors for managing the resource's lifecycle.
  - The `lifecycle` block is optional but powerful for managing resource behavior.
  - `create_before_destroy` is useful for minimizing downtime.
  - `prevent_destroy` is critical for protecting important resources.
  - `ignore_changes` is handy for ignoring external or non-critical changes.
  - `replace_triggered_by` ensures resources are recreated when dependent attributes change.
- difference between ansible and terraform
  - if your infrastructure is like evolving over time like installation of new softwares, upgrade activities than ansible excels in that 
  - but if you want to provision complex infrastrastructure than terraform is best
  - so choice of iac tool should be based on specific requirement
- let's say there are 20 resource deployed using terraform and they are running so i want to delete only 1 or 2 resource how to do that in terraform 
  - command :  terraform destroy -target=<resource>.<name>
- what is module
  - it is package of multiple resources that we can reuse
- what are different kinds of modules
  - root module, 
    - The root module is the main working directory where we runs terraform commands 
  - child module
    - child module are modules that called by root modules
  - publish module
    - we can publish any module to terraform registry and call in our root module is called published module
- let's say you want to get public ip for ec2 instance from output how to get that 
- terraform workspaces
  - it stores different state files and configurations files
  - terraform workspace select <workspace-name>



- https://developer.hashicorp.com/terraform/tutorials/state/resource-drift
- https://www.youtube.com/watch?v=t9bHZMFxQYY&ab_channel=LogicOpsLab


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
  - autoscaling group 
  - launch configurations
  - scaling policy  
- route table 
  - subnet association 
- internet gateway 
- net gateway 
- vpn
- direct connect
- Load Balancers ( types )
  - 4 types
    - Application
    - Network 
    - Classic
    - Gateway LoadBalancer
      - Choose AWS Gateway Load Balancer for easy integration with security and network tools, automatic traffic distribution, and improved performance and reliability of your applications
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
- Different types of LoadBalancer Service
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
- what are the majour feature of docker


## CICD 
- Jenkins
  - what is declarative pipeline 
  - how to add agents in Jenkins 
  - what is Jenkins shared library 
  - how to run parallel jobs in Jenkins 
  - how to store sensitive information in Jenkins 
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
- Booting process
- sed command
- find command
- grep command
- awk command
- netstat
- protocoals

## Ansible
- what is default path for hosts 
- how to check host is accessible or not 
- ansible facts 
- 


## Prometheus, Grafana, loki, elk stack 
- promql 
- elk configuration, efk configuration 
- created custom dashboards 


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
