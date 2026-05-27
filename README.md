# 🚀 terraform-aws-networking-lab

**Production-grade AWS networking infrastructure as code** — part of the DevEmpire2026 revival.

This repo contains reusable Terraform modules for building secure, scalable, and highly available network foundations on AWS.

## ⚡ What’s Inside
- VPC with public/private subnets across multiple AZs
- Internet Gateway + NAT Gateways
- Security Groups (web, app, db tiers)
- Route tables + custom routing
- NACLs + flow logs enabled
- Outputs for easy integration with other infrastructure

## 🔧 Tech Stack
- Terraform 1.8+
- AWS Provider
- Standard module structure (variables, outputs, main.tf)

## 🚀 Quick Start
```bash
git clone https://github.com/Lluminatarion-8431/terraform-aws-networking-lab.git
cd terraform-aws-networking-lab
terraform init
terraform plan
terraform apply
```

## 📈 Architecture
```
[Internet] → IGW → Public Subnets (ALB)
                  ↓
             Private Subnets (App + DB)
                  ↓
             NAT Gateway (Egress)
```

## 🎯 Next Steps
- Add Transit Gateway support
- Implement VPC Peering modules
- Add Direct Connect / VPN options
- Integrate with EKS / ECS networking

**Built for real production use. Clean. Reusable. Scalable.**

---

🔥 Part of [DevEmpire2026](https://github.com/Lluminatarion-8431/DevEmpire2026) | Network Engineering & DevOps Portfolio