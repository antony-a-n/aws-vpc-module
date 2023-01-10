This is a basic terraform code for creating a AWS VPC, which includes IGW,NATGW,public &private subnets nad it's route table associations .The number of subnets are will be based on the no of avaliability zones on the provided region.And the subnetting will be carried out based on the built-in function **cidrsubnet**.

The internet access to priavte subnets are setup with help of NATGW and it is a optional feature.By default is is set as **true**.Regardless of the status of NAT gateway,the priavte subnets will be associated with the priavte route table.

Based on this VPC module, I have created a multi-tier wordpress deployment and you can find the repository [here](https://github.com/antony-a-n/multi-tier-wordpress-deployment-with-terraform/).

