### Set up AKS with CloudFormation script    


#### Prerequisites

1. AWS CLI v1.18.133 or later (`aws --version`)
2. AWS CLI credentials configured
3. `kubectl` installed and added to your path (command-line utility for communicating with the cluster API server)

#### Steps prior to cluster creation

1. Create Amazon EKS cluster IAM role (including creating a stack)
    - Follow steps to upload file (`iam.yaml`) to the CloudFormation console: https://docs.aws.amazon.com/eks/latest/userguide/getting-started-console.html#role-create

2. Create Amazon EKS cluster VPC
    - Follow steps to upload file (`amazon-eks-vpc-private-subnets.yaml`) to the CloudFormation console: https://docs.aws.amazon.com/eks/latest/userguide/getting-started-console.html#vpc-create

#### Application Architecture

<img src="images/EKS-demo-app.png" width="600">

Taken from tutorial:
https://docs.aws.amazon.com/eks/latest/userguide/getting-started-console.html