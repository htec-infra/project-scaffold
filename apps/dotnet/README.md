# Terraform module generator

Scaffolding for new dotNet projects

### Features
- infra - Boostrap scripts and infrastructure-related definitions 
  (Dockerfile,k8s manifests, helm charts, etc.)
- src - Main projects (the product code)
- tests - Test projects
- docs - Documentation stuff, markdown files, help files etc.
- samples (optional) - Sample projects
- lib - Things that can NEVER exist in a nuget package
- artifacts - Build outputs go here. Doing a build.cmd/build.sh generates artifacts here (nupkgs, dlls, pdbs, etc.)
- packages - NuGet packages

### Prerequisites

- [pre-commit](https://pre-commit.com/#install)

