---
description: Description of files and folders used by terraform
---

# Files/Folders

## Common Practice Files

The following files are list of commonly used file names and their general purpose.

* locals.tf - Used to define local variables
* main.tf - Majority of the code that is executed to deploy resources
* ouput.tf - Used for defining the values that will be outputed to be viewed during/after applying
* variables.tf - Used to define input variables

## .terraform.lock.hcl

Contains provider version information

{% embed url="https://developer.hashicorp.com/terraform/language/files/dependency-lock" %}

## tfvar files

Files used to assign variables:

* \*.auto.tfvars
* \*.auto.tfvars.json
* terraform.tfvars.json
* terraform.tfvars

For order of precedence see [Variables in HCL](../hcl.md#order-of-precedence-for-variable-assignment).

