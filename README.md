# Terraform Module: AWS S3 Bucket

This Terraform module creates an S3 bucket on AWS every time Terraform is run.

## Prerequisites

- Terraform installed locally. You can download Terraform from [here](https://www.terraform.io/downloads.html).
- AWS account credentials configured locally. You can set up your AWS credentials using the AWS CLI or by setting environment variables.

## Usage

```hcl
module "s3_bucket" {
  source  = "github.com/your_username/terraform-aws-s3-bucket"

  bucket_name = "my-unique-bucket-name"
  region      = "us-east-1"
  acl         = "private"
  force_destroy = true
}
