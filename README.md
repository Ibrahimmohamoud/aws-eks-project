# AWS EKS Project

## Structure
```
aws-eks-project/
├── terraform/
│   ├── main.tf
│   ├── provider.tf
│   ├── variables.tf
│   └── outputs.tf
├── app/
│   └── main.py
├── .github/workflows/
│   └── deploy.yml
└── README.md
```

## Usage

1. Configure your AWS credentials.
2. Set required Terraform variables (see `terraform/variables.tf`).
3. Run Terraform to provision EKS:
   ```sh
   terraform -chdir=terraform init
   terraform -chdir=terraform apply
   ```
4. Deploy the app to EKS (see `.github/workflows/deploy.yml`).