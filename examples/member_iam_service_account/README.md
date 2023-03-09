# Member iam Module Example

This example illustrates how to use the `member_iam` submodule

## Requirements
### Installed Software
- [Terraform](https://www.terraform.io/downloads.html) 
- [Terraform Provider for GCP](https://github.com/terraform-providers/terraform-provider-google) 
- [Terraform Provider for GCP Beta](https://github.com/terraform-providers/terraform-provider-google-beta) 

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| project\_id | Project id | `string` | n/a | yes |
| account\_id  | Account id of service account to be created | `string` | n/a | yes |
| display\_name | Display name of service account | `string` | n/a | yes |
| project\_roles | List of roles to be assign to new service account | `list(string)` | n/a | yes |


## Outputs

| Name | Description |
|------|-------------|
| project\_id | Project id. |
| roles | Project roles. |
| service\_account\_address | Member which was bound to projects. |

## Usage
To run this you need to execute:

```
$ terraform init
$ terraform plan -var-file=var.tfvars
$ terraform apply -var-file=var.tfvars
```

**Note:** Modify the variable's values in **"var.tfvars"** file according to the requirements. 