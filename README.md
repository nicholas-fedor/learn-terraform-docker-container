# Terraform Get Started with Docker

[Tutorial for HashiCorp's
Terraform](https://developer.hashicorp.com/terraform/tutorials/docker-get-started)

## Notes

This is a tutorial that can be used to get started using Terraform on a local
instance of Docker running on WSL.

The original documentation references the following Docker provider
configuration in main.tf:

```console
provider "docker" {  host    = "npipe:////.//pipe//docker_engine"}
```

This doesn't work for when Docker is running out of WSL. Instead, use the
following:

```console
provider "docker" {}
```
