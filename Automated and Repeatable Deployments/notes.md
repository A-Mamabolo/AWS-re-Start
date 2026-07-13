# Automated and Repeatable Deployments Notes

## Automated Deployments
Automated deployments reduce manual configuration and ensure resources are deployed consistently every time.

## AMI Building Strategy
An Amazon Machine Image (AMI) is a template used to launch EC2 instances.

## EC2 Launch Templates
Launch Templates store instance configuration settings such as:

* AMI ID
* Instance type
* Security groups
* Storage configuration
* Key pairs

Benefits:
* Consistency
* Reusability
* Simplified Auto Scaling deployments

## Infrastructure as Code (IaC)
Infrastructure as Code allows infrastructure to be managed using code instead of manual configuration.

Benefits:
* Version control
* Automation
* Repeatability
* Reduced errors

## JSON and YAML
CloudFormation templates can be written using:

### JSON
JavaScript Object Notation

### YAML
YAML Ain't Markup Language
YAML is generally easier to read and write.

## AWS CloudFormation
AWS CloudFormation is a service that provisions AWS resources using templates.

Key Features:
* Automates infrastructure deployment
* Supports version-controlled templates
* Creates repeatable environments
* Integrates with many AWS services

Common Resources:
* EC2 Instances
* VPCs
* Security Groups
* S3 Buckets
* IAM Roles

## Key Takeaways
* Infrastructure should be automated whenever possible.
* Launch Templates standardize EC2 deployments.
* CloudFormation enables Infrastructure as Code.
* JSON and YAML are commonly used template formats.
* Automation improves consistency and reduces operational risk.
