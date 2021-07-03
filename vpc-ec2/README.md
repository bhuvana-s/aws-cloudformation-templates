Two CloudFormation Templates to create the following AWS Resources.

1. vpc-demo.yaml - 
   -> deploys a VPC, with a pair of public and private subnets spread across two Availability Zones. 
   -> It deploys an internet gateway, with a default route on the public subnets. It deploys a pair of NAT gateways (one in each AZ), and default routes for them in the private subnets.
   -> It deploys an EC2 security group for the instance to give you SSH access

 2. ec2-linux-demo.yaml -
   -> Create an Amazon EC2 instance running the Amazon Linux AMI. The AMI is chosen based
  on the region in which the stack is run.