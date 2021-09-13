# Terraform module generator

Scaffolding for new dotNet-core projects

### Features
- docs - Documentation stuff, markdown files, help files etc.
- infra - Boostrap scripts and infrastructure-related configuration templates 
  (Dockerfile,k8s manifests, helm charts, etc.)
- libs - All third-patry dependencies that can't be pulled from NuGet repo, place here
- src - Main projects (the product code)
- tests - Project's test suites
- samples (optional) - Sample projects
- artifacts - Build outputs go here. Doing a build.cmd/build.sh generates artifacts here (nupkgs, dlls, pdbs, etc.)
- packages - NuGet packages

### Prerequisites

- [pre-commit](https://pre-commit.com/#install)
- [skaffold](https://skaffold.dev/docs/install/)

### Installation

### Usage


### Credits

    https://github.com/dotnet/aspnetcore
