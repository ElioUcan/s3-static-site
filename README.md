# S3 Static Site

A personal profile page hosted as a static website on AWS S3, provisioned with Terraform.

## Overview

A simple HTML/CSS page deployed to an S3 bucket configured for static website hosting. The infrastructure is fully managed as code — one `terraform apply` and the site is live.

## Tech Stack

- **HTML/CSS** — static front-end
- **AWS S3** — static website hosting
- **Terraform** — infrastructure as code (`infra/`)

## Infrastructure

The `infra/` directory contains:

| File | Description |
|------|-------------|
| `main.tf` | S3 bucket, bucket policy, and website configuration |
| `variables.tf` | Configurable inputs (bucket name, region, etc.) |
| `outputs.tf` | Website endpoint URL |

## Deploy

```bash
cd infra
terraform init
terraform apply
```
