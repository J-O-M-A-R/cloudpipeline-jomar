# cloudpipeline-jomar
# IAC Demo - README

**What this does**
- Creates an AWS VPC, one public subnet, and an Internet Gateway.
- Adds a security group allowing HTTP (80) and SSH (22).
- Generates an SSH key pair (saved locally).
- Launches one Amazon Linux 2 EC2 instance with Apache and a simple index page.

**Files**
- iac/main.tf — Terraform code to create the resources.

**Quick commands**
1. terraform init
2. terraform plan
3. terraform apply
4. Visit: http://<instance_public_ip> (see terraform output)
5. Cleanup: terraform destroy

**Notes**
- The generated private key is saved as `iac-demo-key.pem` in the same folder—add it to `.gitignore`.
- Replace region or instance type as needed for your sandbox limits.
- This is minimal and intended for learning.
