# Terraform-Azure-Static-Websit
Hosting a static website using Azure storage account
## Step-01: Execute Terraform Commands 
```t
# Terraform Initialize
terraform init

# Terraform Validate
terraform validate

# Terraform Format
terraform fmt

# Terraform Plan
terraform plan

# Terraform Apply
terraform apply -auto-approve

## Step 2: Upload Static Content
1. Go to Storage Accounts -> staticwebsitexxxxxx -> Containers -> $web
2. Upload files from folder "static-content"

## Step 3: Verify 
1. Azure Storage Account created
2. Static Website Setting enabled
3. Verify the Static Content Upload Successful
4. Access Static Website: Goto Storage Account -> staticwebsitexxxxx -> Data Management -> Static Website
5. Get the endpoint name `Primary endpoint`
https://staticwebsitetxeril.z13.web.core.windows.net/

## Step-04: Destroy and Clean-Up
# Terraform Destroy
terraform destroy -auto-approve

# Delete Terraform files 
rm -rf .terraform*
rm -rf terraform.tfstate*
