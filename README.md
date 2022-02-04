### terraform-aws-keypair

### Please copy paste below code
```
module "dev"{
    source = "Maksym83/keypair/aws"
    region = "us-east-1"
    key_name_prefix = "dev-"
    key_location
}
output region{
    value =module.dev.region
    output key_name{
        value = module.dev.key_name
    }
```