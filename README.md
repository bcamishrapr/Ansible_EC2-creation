# EC2_Instance_Create

This Playbook is used to install EC2-instance in us-east-1 region.

** Prequisite **
-- sudo yum install python2-boto.noarch -y
-- sudo yum install python-boto3.noarch (For connecting with AWS-account)
-- Need to create one IAM user in AWS-account with programmtic-access.
-- then export secret-access-key , access-key-id in control machine like  below.
== export AWS_ACCESS_KEY_ID='453A'
== export AWS_SECRET_ACCESS_KEY='irgg'

Note:-- key-pair should be in same region in which instances is going to create.
--TO Run specific Tasks inside the playbook we use tags which should be already defined in playbook.

==> ansible-playbook ec2_create.yml --tags "packages"
