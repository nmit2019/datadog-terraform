## Terraform code for Datadog synthetic test that will monitor Website & alert on slack

Terraform code can be used to created Datadog syncthetic test to monitor any public facing website and status will be displace on Datadog dashboard

## Usage

```hcl
        module "webiste-monitoring" {
            source = "github.com/nmit2019/datadog-terraform?ref=master"
            website-name = var.website-name
            aws_regions = var.aws_regions
            testing_frequency = var.testing_frequency
            slack_channel_name = var.slack_channel_name
            tags = var.tags
        }
        
```
