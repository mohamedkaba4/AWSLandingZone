### Mavencrest AWS Multi-Account Landing Zone

AWS multi-account landing zone designed to provide secure, scalable, and governed cloud environments using Infrastructure as Code.

It has a shared platform layer for management groups, policies, monitoring, security, and hub networking, plus a separate production workload repo for the prod spoke VNet, subnet, NSG, and hub-spoke peering. (Deployed with ALZ Accelerator working as a template)

Terraform state is centrally stored in Azure Storage, with separate state files for the platform and workload environments. Azure Policy is actively enforcing standards, and CI/CD is being set up with separate plan and apply identities using workload identity federation and least-privilege RBAC.

## Scope

- AWS Organizations and multi-account structure
- Organizational Units (OU) hierarchy
- Service Control Policies (SCPs) and governance guardrails
- Centralized logging and monitoring
- Security and workload account separation
- IAM and cross-account access
- Terraform-based Infrastructure as Code
- GitHub Actions with OIDC
- Workload account onboarding

