# Victor Rodriguez Final Project

This final project uses an AWS account and Terraform to create a VPC with public and private subnets.

## Requirements

- AWS Account

This project requires an AWS account and the setup of an organization and users through AWS Organizations and IAM respectively.

- Terraform

This project uses Terraform, an infrastructure-as-code tool, to create and manage the VPC and its subnets in AWS.

## Required program installations

1. Install AWS CLI
Go to the official website https://aws.amazon.com/es/cli/ and download the respective intaller.
You can check the version by running the following command in the console:

```console
aws --version
```

2. Install Terraform
Go to the official website https://developer.hashicorp.com/terraform/install?product_intent=terraform and download the respective intaller or use a command.
You can check the version by running the following command in the console:

```console
terraform --version
```

Additionally, you can install an extension for your text editor.

## Usage

Once you have cloned the project, and accessed AWS from an alternate account to the root one, consider using the following commands, taking care of the passwords of your AWS account.

1. `terraform init`: This command initializes your working directory with the files necessary to run Terraform. In the context of AWS, this might involve setting up your AWS provider and downloading the necessary modules to create a VPC.

2. `terraform validate`: This command checks the syntax of your Terraform configuration files and confirms that they are well formed. This is useful for ensuring that your VPC and subnet definitions are correct before attempting to apply them.

3. `terraform plan`: This command creates an execution plan that shows what actions Terraform will perform on your AWS infrastructure. This allows you to review the changes that will be made to your VPC and subnets before applying them.

4. `terraform apply`: This command applies the changes described in your execution plan. This could involve creating a new VPC and subnets, or modifying existing ones.

5. `terraform destroy`: This command destroys the resources that Terraform has created. In the context of a VPC, this would delete the VPC and all associated subnets.

Please note that these commands must be executed in the mentioned order to ensure a correct workflow. 😊

## License

The project is under the ©MIT License.
