Terraform module to provision an EC2 instance that is running Apache.
Not intended for production use. Just showcasing how to create a custom public module on Terraform Registry.

```hcl
module "apache" {
    source = ".//terraform_aws_apache_example"
    vpc_id= "vpc-000000000"
    my_ip = "MY_OWN_IP_ADDRESS/32"
    public_key = "ssh-rsa AAAAB..."
    instance_type = "t2.micro"
    server_name = "Apache Example Server"
}

output "public_ip" {
  value = module.apache.public_ip
}
```


