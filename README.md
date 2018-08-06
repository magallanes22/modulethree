## ModuleThree
1. Create an AWS IAM role
2. Create an S3 bucket as input data for the web application


### Requirement:
Need a terraform.tfvars file with AWS creds and private key path

```
$ cat ../terraform.tfvars 
aws_access_key = "your-aws-access-key"
aws_secret_key = "your-aws-secret-key"
private_key_path = "/Users/username/aws/keys"
key_name  = "your-aws-ssh-privatekey-filename"
```
### Terraform commands:
```
terraform plan -var-file='../terraform.tfvars'
terraform apply -var-file='../terraform.tfvars'
terraform destroy -var-file='../terraform.tfvars'
```
.

