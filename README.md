# aws-service_ansible
Creating EC2 instance in AWS through ansible using boto library.

##### AWS credentials configured at below path.
```
~ /.aws/credentials
```
##### No Inventory file is required as we are using :
```
connection= local
```

##### We can run the playbook using tags used.

```
ansible-playbook awsservices.yml --tags ec2
```
###### OR
```
ansible-playbook awsservices.yml --tags s3 --extra-vars "s3state=present"
```
