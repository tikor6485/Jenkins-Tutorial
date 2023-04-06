Jenkins-Tutorial on AWS

This repository contains code and resources related to a tutorial on setting up Jenkins on AWS using Ansible. The tutorial walks through the process of launching an EC2 instance on AWS, configuring it with Ansible, and installing and configuring Jenkins on the instance.
Contents

    ansible/: Contains Ansible code for configuring the EC2 instance and installing Jenkins.
    terraform/: Contains Terraform code for launching the EC2 instance on AWS.
    docs/: Contains documentation related to the tutorial.

Requirements

    AWS account
    Terraform 0.14.x
    Ansible 2.9.x
    AWS CLI

Usage

    Clone this repository to your local machine.
    Navigate to the terraform/ directory and run terraform init to initialize the Terraform modules.
    Create a terraform.tfvars file with your AWS access key and secret key.
    Run terraform apply to launch the EC2 instance on AWS.
    Navigate to the ansible/ directory and run ansible-playbook -i inventory.ini jenkins.yml to configure the instance and install Jenkins.
    Access the Jenkins UI by navigating to http://<EC2-Instance-Public-IP>:8080 in your web browser.

Contributing

Contributions to this repository are welcome! If you find a bug or want to add a new feature, please open an issue or pull request.
