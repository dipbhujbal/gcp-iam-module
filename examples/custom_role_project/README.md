# Project Level Custom Role Example

This example illustrates how to use the `custom_role_iam` submodule to create a custom role at the project level.

## Requirements
### Installed Software:
- [Terraform](https://www.terraform.io/downloads.html) 
- [Terraform Provider for GCP](https://github.com/terraform-providers/terraform-provider-google) 
- [Terraform Provider for GCP Beta](https://github.com/terraform-providers/terraform-provider-google-beta) 


## Inputs Variables



| Name    | Description | Type | Default | Required |
|--------|:-------------:|:------:|:---------:|:--------:|
| project\_id | Project ID. | `string` | n/a | yes |
| role_id | Role ID | `string` | n/a | yes |
| base_roles | Base roles | `list(string)` | n/a | yes |
| permissions | List of permissions to assign to new role | `list(string)` | n/a | yes |
| excluded_permissions | List of permissions to excluded for new role |  `list(string)` | n/a | yes |
| members | List of members to bind to new custom role |  `list(string)` | n/a | yes


## Outputs

| Name | Description |
|------|-------------|
| role\_id | ID of the custom role created at project level. |

## Usage
To run this you need to execute:

```
$ terraform init
$ terraform plan -var-file=var.tfvars
$ terraform apply -var-file=var.tfvars
```

