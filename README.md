# AWS Github Actions OIDC Provider Terraform Module

This module creates a OIDC Provider configured to allow connection to AWS from Github Actions.

You can then use this to create roles to allow your repositories to access your AWS account.
We have created a separate [terraform-aws-github-actions-oidc](https://github.com/armakuni/terraform-aws-github-actions-oidc) module for this purpose.

<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_iam_openid_connect_provider.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_openid_connect_provider) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_github_thumbprint"></a> [github\_thumbprint](#input\_github\_thumbprint) | GitHub OpenID TLS certificate thumbprint (the default is the current value) | `string` | `"6938fd4d98bab03faadb97b34396831e3780aea1"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_arn"></a> [arn](#output\_arn) | n/a |
<!-- END_TF_DOCS -->
