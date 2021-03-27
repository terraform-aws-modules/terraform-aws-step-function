# Complete AWS Step Function example

Configuration in this directory creates AWS Step Function and IAM role with large variety of supported AWS Service integrations and custom policies.

Note: You probably don't need to set custom/additional policies but use `service_integrations` only.


## Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

Note that this example may create resources which cost money. Run `terraform destroy` when you don't need these resources.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13.1 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 3.27 |
| <a name="requirement_random"></a> [random](#requirement\_random) | >= 2 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 3.27 |
| <a name="provider_random"></a> [random](#provider\_random) | >= 2 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_disabled_step_function"></a> [disabled\_step\_function](#module\_disabled\_step\_function) | ../../ |  |
| <a name="module_step_function"></a> [step\_function](#module\_step\_function) | ../../ |  |

## Resources

| Name | Type |
|------|------|
| [aws_sqs_queue.queue](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [random_pet.this](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/pet) | resource |

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_this_role_arn"></a> [this\_role\_arn](#output\_this\_role\_arn) | The ARN of the IAM role created for the State Machine |
| <a name="output_this_role_name"></a> [this\_role\_name](#output\_this\_role\_name) | The name of the IAM role created for the State Machine |
| <a name="output_this_state_machine_arn"></a> [this\_state\_machine\_arn](#output\_this\_state\_machine\_arn) | The ARN of the State Machine |
| <a name="output_this_state_machine_creation_date"></a> [this\_state\_machine\_creation\_date](#output\_this\_state\_machine\_creation\_date) | The date the State Machine was created |
| <a name="output_this_state_machine_id"></a> [this\_state\_machine\_id](#output\_this\_state\_machine\_id) | The ARN of the State Machine |
| <a name="output_this_state_machine_status"></a> [this\_state\_machine\_status](#output\_this\_state\_machine\_status) | The current status of the State Machine |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
