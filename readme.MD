#custom AWS VPC Module

this module is developed for joindevops.com. we are creating following resources.this module creates resources in first 2 AZ for HA.

. VPC
. internet gateway 
. Internet and VPC attachment
. 2 Public Subnets.
. 2 Private Subnets.
. 2 database Subnets.
. EIP 
. NAT Gateway 
. Public Route Table 
. Private Route Table 
. Database Route Table 
. Route Table Associations
. Routes in all tables 
. Peering if required for user 
. Routes of peering in requestor and            acceptor VPC. 
. Database subnet groups

### inputs ###

. Project name(required) : user should mention project name.Type is string.
. Environment (Optional) : Default value is DEV.type is string.
. common_tags(required): user should provide 

### outputs ###
.vpc_id: vpc_id 
.public_subnet_ids: A list of 2 public subnet IDS ceated
.private_subnet_ids: A list of 2 private subnet IDS ceated
.database_subnet_ids: A list of 2 database subnet IDS ceated
