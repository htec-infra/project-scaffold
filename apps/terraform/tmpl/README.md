# terraform-template

Description

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 3.65 |

## Providers

No providers.

## Modules

No modules.

## Resources

No resources.

## Inputs

No inputs.

## Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Development

### Prerequisites

- [terraform](https://learn.hashicorp.com/terraform/getting-started/install#installing-terraform)
- [pre-commit](https://pre-commit.com/#install)
- [terraform-docs](https://github.com/segmentio/terraform-docs) (needed for pre-commit)
- [tflint](https://github.com/terraform-linters/tflint) (needed for pre-commit)
- [tfsec](https://github.com/aquasecurity/tfsec) (needed for pre-commit)
- [checkov](https://github.com/bridgecrewio/checkov) (needed for pre-commit)
- [golang](https://golang.org/doc/install#install) (needed for Terratest tests)

### Configurations

Configure pre-commit hooks
```sh
pre-commit install
```

### Tests

- Tests are available in `test` directory
- In the test directory, run the below command
```sh
go test
```

## Authors

This project is authored by following people:

-

