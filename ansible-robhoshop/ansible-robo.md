1). Create one t2.micro ec2 instance in aws using aws console
    - install ansible in ec2 instance
        sudo yum install ansible -y
    - Give IAM role to this ec2 instance
        - select ansible ec2 instance and click on actions
        - click on security and select IAM role
        - select the role which you have created

2). Create all ec2 instance for roboshop project using 1-roboshop.sh from shell-roboshop directory

3). Using ansible ec2 we will connect all other roboshop ec2 instances and install the required software
    - # ansible-playbook -i inventory.ini -e ansible_user=centos -e ansible_password=DevOps321 mongodb.yaml