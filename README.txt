Assumptions:
- Remote webserver is on and connected to local server
- Remote webserver's ip is registered in the hosts file
- Undeploying is interpreted as taking down the webserver
- If wanted to use with AWS EC2, would use ansible on top of CloudFormation, but not in scope of this assignment



1. Test Connection: 
ansible -m ping all

2. To deploy webserver:
ansible-playbook deploywebserver.yml

3. To undeploy webserver:
ansible-playbook undeploywebserver.yml
