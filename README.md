# Example App Terraform Module

An example Terraform module repository used to showcase automation and tooling.

## Key Features

- [x] Automatic dependency updates using `dependabot`.
- [x] Automatic release management using `semantic-release`.
- [x] Terraform documentation validation using `terraform-docs`.
- [x] Terraform formatting validation using `terraform fmt`.
- [x] Terraform security checks using `checkov`.
- [x] Terraform linting with `tflint`.
- [x] Ensure required files exist in the repository (for example, CODEOWNERS).

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.1 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | 5.27.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 5.27.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|


## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_bucket"></a> [bucket](#output\_bucket) | The name of the S3 bucket containing the Terraform state file. |
| <a name="output_dynamodb_table"></a> [dynamodb\_table](#output\_dynamodb\_table) | The name of the DynamoDB table handling Terraform state. |
| <a name="output_encrypt"></a> [encrypt](#output\_encrypt) | Whether or not the S3 bucket is encrypted. |
| <a name="output_key"></a> [key](#output\_key) | The name of the state file that will exist in the S3 bucket. |
| <a name="output_kms_key_id"></a> [kms\_key\_id](#output\_kms\_key\_id) | The name of the KMS key used to encrypt the S3 bucket. |
| <a name="output_region"></a> [region](#output\_region) | The AWS region the S3 bucket is deployed to. |
<!-- END_TF_DOCS -->

## Authors
Module is maintained with the help from [these awesome
contributors](https://github.com/craigsloggett-lab/terraform-aws-app/graphs/contributors).

## License
MIT Licensed. See
[LICENSE](https://github.com/craigsloggett-lab/terraform-aws-app/blob/main/LICENSE)
for full details.
