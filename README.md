Terraform Module to provision an AWS EC2 instance with the latest amazon linux 2 ami and installed docker in it.

Not intended for production use. It is an example module.

It is just for showing how to create a publish module in Terraform Registry.

Usage:

```hcl

provider "aws" {
  region = "us-east-1"
  access_key = "AKIA42LO3ELC62VDHJOM"
  secret_key = "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"
}

module "docker_instance" {
    source = "<github-username>/docker-instance/aws"
    key_name = "clarusway"
}