# Terraform Azure AKS 

This repository provisions an AKS cluster in Azure using Terraform modules.

## Structure
- `modules/network`: VNet and Subnet
- `modules/aks`: AKS cluster definition
- `environments/dev|staging|prod`: Environment-specific configurations

## Usage
```bash
cd environments/dev
terraform init
terraform plan
terraform apply
```

## Requirements
- Terraform >= 1.3
- Azure CLI with authenticated session
- Remote state backend configured in `backend.tf`
