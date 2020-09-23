# Overview

* [The AWS Command Line Interface(CLI)](https://aws.amazon.com/cli/) is a unified tool to manage your AWS services.
* These files are my practices about how to control multiple AWS services from the command line and automate them through scripts.



# Pre-Requisites
* [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) 
* [Configure AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html)

# Content

Directory | Tasks | AWS services
------------ | ------------- | -------------
[aws-cli-01-ec2/c01-aws01/afaryy/](./aws-cli-01-ec2/c01-aws01/afaryy/) | Create a jumpbox with a public IP address <br> Creat another EC2 with private address <br> Use jumpbox to connet with it through SSH  | EC2 instance, Security group, Key pair
[aws-cli-02-s3/c01-aws02/afaryy/](./aws-cli-02-s3/c01-aws02/afaryy/) | Create a S3 bucket and upload a file to it <br> Access the file on the S3 bucket from a EC2 instances <br> | S3, IAM, EC2
[aws-cli-02-s3/c04-iam01/afaryy/](./aws-cli-02-s3/c04-iam01/afaryy/) | Create a AMI user with read only access policy to S3 | S3, IAM
[aws-cli-02-s3/c04-s301/afaryy/](./aws-cli-02-s3/c04-s301/afaryy) | Create a bucket, upload a file and expose a website | S3, IAM
[aws-cli-03-vpc/c02-network03/afaryy/](./aws-cli-03-vpc/c02-network03/afaryy/) | Create a new AWS VPC |  VPC
[aws-cli-03-vpc/c02-network04/afaryy/](./aws-cli-03-vpc/c02-network04/afaryy/) | Create 2 subnets (private and public) per Availability Zone |  VPC, Subnets
[aws-cli-03-vpc/c02-network05/afaryy/](./aws-cli-03-vpc/c02-network05/afaryy/) | Create an Internet Gateway and attach it to your VPC |  VPC, Internet Gateway
[aws-cli-03-vpc/c02-network06/afaryy/](./aws-cli-03-vpc/c02-network06/afaryy/) | Create a NAT Gateway attach it to one of your public subnets with an Elastic IP |  VPC, NAT Gateway
[aws-cli-03-vpc/c02-network07/afaryy/](./aws-cli-03-vpc/c02-network07/afaryy/)| Create the route tables and associate with private and public subnets |  VPC, Route Tables
[aws-cli-03-vpc/c02-network08/afaryy/](./aws-cli-03-vpc/c02-network08/afaryy/) | Add inbound and outbound rulesfor Network ACL |  VPC, NACL
[aws-cli-03-vpc/c02-network09/afaryy/](./aws-cli-03-vpc/c02-network09/afaryy/) | Create two new security groups with attached to your new VPC |  VPC, Security Group
[aws-cli-03-vpc/c02-network10/afaryy/](./aws-cli-03-vpc/c02-network10/afaryy/) | Create a new ENI attached to one of your private subnets <br>Give it a fixed IP address within the network range of the chosen subnet |  VPC, ENI, EIP, Subnets
[aws-cli-03-vpc/c02-network11/afaryy/](./aws-cli-03-vpc/c02-network11/afaryy/) | Launch an EC2 instance on a public subnet, attach your public SG to your public instance <br> Launching an EC2 instance on private subnet using custom ENI that private SG attached  <br> Access to your public instance using SSH <br> From the public instance, SSH to your private one <br> From the PRIVATE instance, try to ping 8.8.8.8 to check internet connection through NATGW |  EC2, Security Group, VPC, Subnet, ENI
[aws-cli-03-vpc/c02-network12/afaryy/](./aws-cli-03-vpc/c02-network12/afaryy/) | Pair with someone else or another account and create a VPC peering within your vpc's |  VPC Peering
[aws-cli-04-asg/c03-aws01/afaryy/](./aws-cli-04-asg/c03-aws01/afaryy/) | Create an Auto Scaling Group | Auto Scaling Group
[aws-cli-05-lb/c03-aws02/afaryy/](./aws-cli-05-lb/c03-aws02/afaryy/) | Create an Application Load Balancer  | Load Balancer
[aws-cli-06-route53/c03-aws03/afaryy/](./aws-cli-06-route53/c03-aws03/afaryy/) | Create or use created public hosted zone <br> Create a private or public hosted zone <br>  Create Route53 record associated with created Application Load Balancer <br> Test the friendly records | Route53


# Authors

## Yvonne(Yingying) Yao

- Linkedin: [https://www.linkedin.com/in/yvonneyao/](https://www.linkedin.com/in/yvonneyao/)
- Github: [https://github.com/afaryy](https://github.com/afaryy)
- Member: [DevOps Academy](https://github.com/devopsacademyau)

# Thanks
Thank [DevOps Academy](https://github.com/devopsacademyau) very much.
These files come from my practices for some hands-on labs of AWS CLI on [DevOps Academy](https://github.com/devopsacademyau/academy/tree/master/classes).