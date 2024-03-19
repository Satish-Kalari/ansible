# Installing ansible in ec2 instance
sudo yum install ansible -y

# connecting another ec2 instance with ansible
ansible -i <target ec2 public ip> -e ansible_user=centos -e ansible_password=DevOps1231 -m ping
    - -i: inventory file
    - -e: extra variables
    - -m: module
    - ping: module name



ansible.builtin.yum vs ansible.builtin.package
    - ansible.builtin.yum: This module is used to install, remove, upgrade, update, and list packages and repositories using the YUM package manager.
    - ansible.builtin.package: This module is used to install, remove, upgrade, update, and list packages and repositories using the platform package manager.