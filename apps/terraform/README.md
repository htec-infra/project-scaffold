# Terraform module template

Scaffolding for new Terraform module projects.

### Features

- `main.tf`, `variables.tf`,`outputs.tf` files to module root path

- `.editorconfig`, `.gitignore` and `.terraform-version` files to module root path

- `.pre-commit-config.yaml` for terraform pre-commit git hooks (such as `terraform fmt`, `terraform-docs`, ...)

- `README.md` with an auto-generated section containing Terraform providers, variables and outputs documentation

- `test` directory with an example test (currently using `terragrunt`)

- `example` directory with module usage tf files

### Prerequisites

This is a complete list of CLI tools required to run the full set of pre-commit hooks found in the template. If you would like to omit some tool, make sure to also remove its corresponding hook from the `.pre-commit-config.yaml` file in your own repository.

- [terraform](https://learn.hashicorp.com/terraform/getting-started/install#installing-terraform)
- [pre-commit](https://pre-commit.com/#install)
- [terraform-docs](https://github.com/segmentio/terraform-docs)
- [tflint](https://github.com/terraform-linters/tflint)
- [tfsec](https://github.com/aquasecurity/tfsec)
- [checkov](https://github.com/bridgecrewio/checkov)

You can also try the pre-commit hooks locally with the following command:

```
apps/terraform/tmpl$ pre-commit run --files ./*
```

### Credits

https://github.com/sudokar/generator-tf-module