# Simple Terraform configuration for the latest Ubuntu intance in aws

This repo contains main.tf and data-source.tf, that can be used to build an instance with the latest version of Ubuntu in AWS.

# Prerequisite
You need to have [Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli) installed on you workstation. 

# How to use the repo

* Clone this repo locally to a folder of your choice
```
git clone https://github.com/51r/terraform_aws_instance.git
```

* Make sure you are in the main directory of the repo:
```
cd terraform_aws_instance
```

* initialize Terraform  
```
terraform init
```

* Check the plan in order to see the changes which terraform is going to made.
```
terraform plan
```

* Apply the plan which terraform is going to execute based on our configuration (main.tf)
```
terraform apply
```

* Check the instance build by executing the following command
```
terraform show
```

By the writing of this guide, the latest available version is ubuntu-jammy-22.04-amd64-server.

NOTES: Keep in mind that this will install the latest amd64 version of Ubuntu, available in the AWS Ubuntu owner (099720109477).
