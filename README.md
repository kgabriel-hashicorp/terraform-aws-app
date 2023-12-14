# Example App Terraform Module

This repository contains the standards we recommend having for a child module in Terraform.

## Usage
This terraform module will create an S3 Bucket.

## Module Version Updates

* This module relies on dependabot to manage the module dependencies.
* A PULL REQUEST will automatically be raised if there are new versions of the child modules from either the public or private Terraform Registry.
* The PULL REQUEST will have to approved by the CODEOWNERS.
* More details can be found under ` .github/workflows/README.md `

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
| [aws_dynamodb_table.terraform_state_locks](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/dynamodb_table) | resource |
| [aws_s3_bucket.terraform_state](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket_acl.terraform_state_acl](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/s3_bucket_acl) | resource |
| [aws_s3_bucket_public_access_block.terraform_state_public_access_block](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/s3_bucket_public_access_block) | resource |
| [aws_s3_bucket_server_side_encryption_configuration.terraform_state_sse](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/s3_bucket_server_side_encryption_configuration) | resource |
| [aws_s3_bucket_versioning.terraform_state_versioning](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/resources/s3_bucket_versioning) | resource |
| [aws_caller_identity.current](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/data-sources/caller_identity) | data source |
| [aws_region.current](https://registry.terraform.io/providers/hashicorp/aws/5.27.0/docs/data-sources/region) | data source |

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

## Reference

Link to the [ModuleStandardizationPage]

## Module Dependencies

* This module relies on dependabot to manage the module dependencies.
* A PULL REQUEST will automatically be raised if there are new versions of the child modules from either the public or private Terraform Registry.
* The PULL REQUEST will have to approved by the CODEOWNERS.
* More details can be found under ` .github/workflows/README.md `

## Release Management

* Following [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) a new release is created depending on the PR title prefix and commits.
* The list of allowed PR title prefix can be found [here]



* Root Modules that have dependabot setup for this child module will automatically get the new versions via a PR.


## Contributing

* Commit messages and PR titles must follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
* Pull requests will need to be reviewed by the CODEOWNERS.

## Maintainers

CODEOWNERS file contain the maintainers of this repository
This can also include a link to a [Slack] Channel 

[here]: (https://github.com/kgabriel-hashicorp/terraform-aws-app/blob/47f7be48041bdda79795456c38e3a1d9224d541c/.github/workflows/validate.yml#L22)