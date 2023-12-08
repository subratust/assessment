# assessment
Batch4-8Dec23

## Assessment 1[utilize this in assessment 2]:
    
Imagine you are a DevOps engineer responsible for managing the infrastructure of a new project. The project requires the creation of multiple AWS VPCs, each with its own set of subnets and specific configurations. You need to design a Terraform configuration that can be easily customized for different environments (e.g., development, testing, production).

Question:

VPC Creation:

Design a Terraform configuration to create an AWS VPC with the following specifications:
CIDR block: 10.0.0.0/16
Tags: { Name = "my-vpc", Environment = "dev" }
Customization for Environments:

Implement a way to easily customize the VPC configurations for different environments (dev, test, prod) using Terraform workspaces.
Modularization:

Provisioning Subnets:

Extend your Terraform configuration to provision subnets within the VPC. Each subnet should have a unique CIDR block, and the number of subnets should be configurable.
Dynamic Blocks:

Utilize dynamic blocks to allow dynamic configuration of subnets, taking into account factors like availability zones.
Workspace Usage:

Demonstrate the use of Terraform workspaces to manage different environments. Apply your configuration for both development and production workspaces.
Output and Verification:

Implement output variables to display relevant information, such as the VPC ID and subnet details. Provide commands to verify the outputs after applying the Terraform configuration.

-----------------------------------------------


## Assessment 2: Terraform Advanced Concepts Workshop

You are participating in a hands-on Terraform workshop designed to deepen your understanding of advanced Terraform concepts. In this scenario-based question, you'll navigate through a series of tasks, applying your Terraform skills to real-world scenarios.

Task 1: Setting Up and Version Control
Imagine you are starting a new Terraform project for a cloud infrastructure.

Create a directory structure for the project.
Initialize a Git repository and commit the initial project structure.

Task 2: Module Creation - VPC Configuration
Your team frequently deploys Virtual Private Clouds (VPCs) on AWS, and you want to streamline this process using Terraform modules.

Develop a reusable Terraform module for an AWS VPC with configurable parameters.
Include input and output variables to enhance the module's flexibility and reusability.

Task 3: Main Configuration
In the main Terraform configuration, integrate the VPC module to create a fully-fledged VPC environment.

Define additional resources such as security groups and subnets within the VPC.

Task 4: Provisioners and Remote Execution
As part of your application deployment, you need to install a specific software package on an EC2 instance.

Apply a provisioner to the EC2 instance to accomplish this task.

Task 5: Import Existing Resources
You recently discovered that there is an existing EC2 instance deployed outside of Terraform, and you need to manage it within your Terraform project.

Use terraform import to bring the existing EC2 instance under Terraform management.

Task 6: Remote State Configuration
To enhance collaboration and state management, set up a remote backend using AWS S3 and DynamoDB.

Configure your Terraform project to store the state remotely.
Implement DynamoDB as a state lock to prevent conflicts during concurrent executions.

Task 7: Advanced Module Use - Multi-Tier Application
You are tasked with deploying a multi-tier application stack consisting of a web server and a database.

Develop an advanced module for the multi-tier application stack.
Utilize input variables, outputs, and demonstrate dependencies within the module.

Task 8: Combining Modules for a Complete Environment
Combine the VPC module and the multi-tier application module to deploy a comprehensive environment.

Showcase the ability to compose and reuse modules to create complex infrastructures.

Validate the deployed infrastructure against expected specifications.

Task 10: Destroy Resources and Cleanup
After successfully testing your infrastructure, follow the proper procedures to destroy the deployed resources and clean up the environment.

