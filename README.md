# CloudBreakHDP
Automated Hadoop Cluster ansible / salt script
prerequisites:
1. IAM role
2. Cloudbreak instance with: attached role, public IP, and at least 50Gb storage.

for ansible:
1. place cloudbreak instance IP to inventory file
2. run command: ansible-playbook -i inventory --private-key=$pathtoyourkey.pem cloudbreak.yml
3. run command: ansible-playbook -i inventory --private-key=$pathtoyourkey.pem hadoop.yml
