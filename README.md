aws-vpc-nat-gateway
=============
Create a VPC with Public subnet & Private subnet at Amazon Web Services AWS and enable NAT gateway for Private Subnet

Requirements
------------
- AWS account and credentials

## Role Variables


##### List of Variables

    ---
    region: required
    cidr: required
    public_subnet: required
    private_subnet: required
    public_subnet_az: required
    private_subnet_az: required

##### Example of Variables file
    ---
    
    cidr: 10.22.0.0/16
    public_subnet: 10.22.0.0/24
    private_subnet: 10.22.1.0/24
    public_subnet_az: us-east-1b
    private_subnet_az: us-east-1d


Example Playbook
----------------

##### Simple

    ---
    - hosts: local
      connection: local
      sudo: no
      gather_facts: yes

     roles:
      - vishnudxb.aws-vpc-nat-gateway


License
-------

MIT

Author Information
------------------
Some useful stuff at:
  - [https://github.com/vishnudxb](https://github.com/vishnudxb)
  - Any issues, pull-request are welcome
