# Project Example

This example illustrates how to use the `projects_iam` submodule

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| project\_one | First project id to add the IAM policies/bindings | `string` | n/a | yes |
| sa\_email | Email for Service Account to receive roles (Ex. default-sa@example-project-id.iam.gserviceaccount.com) | `string` | n/a | no |
| user\_email | Email for group to receive roles (Ex. user@example.com) | `string` | n/a | yes |

## Outputs

No output.


## Usage
To run this you need to execute:

```
$ terraform init
$ terraform plan -var-file=var.tfvars
$ terraform apply -var-file=var.tfvars
```
**Note:** Modify the variable's values in **"var.tfvars"** file according to the requirements. 