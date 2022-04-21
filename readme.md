# Terraform Example

## สิ่งที่ต้องมี

1. gcloud sdk บนเครื่อง
2. gcloud authentication
3. gcloud project

## วิธีการใช้งาน

1. Generate ssh key file

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

2. Change your config setting in "terraform.tfvars"

```
project_id = "futureskillstaging"
region     = "asia-southeast1"
zone       = "asia-southeast1-b"
ssh_public_key_filepath  = "ubuntu.pub"
```

3. run terraform

```
terraform plan
terraform init
```
