# AWS Terraform Web Server

This project provisions a basic AWS web server using Terraform, running Apache2. It demonstrates infrastructure as code by provisioning a VPC, subnet, security groups, and an EC2 instance in AWS.

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Setup Instructions](#setup-instructions)
   - [Clone the Repository](#clone-the-repository)
   - [Initialize Terraform](#initialize-terraform)
   - [Apply the Terraform Configuration](#apply-the-terraform-configuration)
   - [Access the Web Server](#access-the-web-server)
3. [Outputs](#outputs)
4. [Screenshots](#screenshots)
5. [License](#license)

---

## Prerequisites

Before running the Terraform configuration, ensure you have the following installed:

1. **Terraform**: Install Terraform by following the instructions [here](https://www.terraform.io/downloads.html).
2. **AWS CLI**: Configure the AWS CLI with access to your AWS account. Follow the guide [here](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html).

---

## Setup Instructions

### 1. Clone the Repository

Clone this repository to your local machine:

git clone https://github.com/Neo9Phoenix/AWS-Terraform.git
cd AWS-Terraform

### 2. Initialize Terraform
Initialize Terraform to download the required provider plugins:
terraform init

### 3. Apply the Terraform Configuration
Provision the infrastructure by running:
terraform apply
Terraform will display the resources it plans to create (e.g., VPC, EC2 instance, security group). Type yes to confirm and apply the changes.

### 4. Access the Web Server
Once the infrastructure is provisioned, Terraform will output the public IP address and URL for the web server. Access the deployed web server by opening a browser and navigating to the provided URL (e.g., http://<public-ip>).
Example: Once your server is up, you should see a page with the message:
your very first web server
This indicates that the Apache web server is successfully running and accessible from the internet.

---

## Outputs 

After running terraform apply, the following details will be shown:
Output Description
Public IP	The public IP of your EC2 instance.
Web Server URL	The URL to access the Apache web server.

---

## Screenshots

Check the screenshots/ folder for screenshots showing the deployed infrastructure, such as the VPC, EC2 instance, and security group configuration.

---

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
