# DevOps exercise AWS: Infrastructure-As-Code

## Introduction

AWS resources and infrastructure should always be created using a configuration management system such as [Terraform](https://www.terraform.io/) or [Cloudformation](https://aws.amazon.com/cloudformation/). This ensures all created AWS resources are tracked and reinstallable.  It also encourages sharing and collaboration and can help an infrastructure recover from a disaster.

## Exercise

1. Install one AWS EC2 Linux instance using either Terraform (preferred) or AWS Cloudformation.
2. Make the instance public available but keep the instance as secure as possible.
3. Pre-install docker software on the instance. Run the  [Apache docker image](https://hub.docker.com/_/httpd/) and make the endpoint public available.
4. Outputs: The configuration code should output the public endpoint of the created service.
5. Document how to create and how to destroy the AWS resources.

## Acceptance Criteria

* The solution is completely installable using the chosen configuration management system.
* The Apache Endpoint is callable from the Internet.
* The solution is as secure as possible.
* All resources can be cleaned up (destroyed) with the chosen configuration system.

## Guidelines/Hints

* Create the EC2 instance with type `t2.micro` or `t2.nano`
* Use your own private AWS account to test the installation (EC2 instance qualifies for free-tier)
* Use an official **Amazon Linux AMI** owned by Amazon.
* You can either install resources without specifying a specific VPC/subnet **OR** install resources in a new VPC/subnet created with the configuration management system

## How to contribute your solution:

1. Fork the repo
2. Commit everything that you do in your fork
3. Create a pull request with your solution. Your pull request should include all source code which you used to create your solution.
4. Provide meaningful comments with your commits
