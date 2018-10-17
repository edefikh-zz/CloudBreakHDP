# CloudBreakHDP
Automated HortonWorks Hadoop Cluster ansible / salt script. This script will run on existing Centos based OS and will install 
CloudBreak 2.7.1 , the second script allows creation of 3 node Hadoop cluster using BluePrints. 
Version 2.6 and 3.0 of HDP is supported.
You can use custom AMI for CloudBreak setup but have to use HDP AMIs for deploying Cluster.

prerequisites:
1. IAM role
2. Cloudbreak instance with: attached role, public IP, and at least 50Gb storage.

for ansible:
1. place cloudbreak instance IP to inventory file
2. run command: ansible-playbook -i inventory --private-key=$pathtoyourkey.pem cloudbreak.yml
3. run command: ansible-playbook -i inventory --private-key=$pathtoyourkey.pem hadoop.yml
