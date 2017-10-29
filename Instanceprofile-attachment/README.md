ANSIBLE PLAYBOOK TO ATTACH ROLE TO AN EC2 INSTANCE
===============================================================================
### Platform
Ansible
### Authors
akhil.baby@reancloud.com

### Implementation
This playbook is to reload sudoers configuration file for the group entries
### Pre-requisites and Dependencies
* Python 2.7.5
* ansible 2.2.0.0
* pexpect 3.3 
   
## Usage Information
Installation

* install the epel-release RPM if needed on CentOS, RHEL, or Scientific Linux
$ sudo yum install ansible

* Ubuntu machines
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible

How to execute playbook

Inorder to get the instanceid's of the instances without the IAM roles execute the script provided which will create a fie instanceid.text.
The playbook contains two roles section one for creating a IAM role and another for attaching the role. If you already have IAM role and just need attaching in this you can just run the profile attachment role in the playbook else you can run both.


Steps
        *Clone the repo to your local machine.
        *Run the ansible playbook with the below command :
                ansible-playbook profile-attachment.yml 

### Release Notes

Initial version of the playbook.

