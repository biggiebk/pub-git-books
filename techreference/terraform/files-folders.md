---
description: Description of files and folders used by terraform
---

# Files/Folders

## .terraform.lock.hcl

Contains provider version information

{% embed url="https://developer.hashicorp.com/terraform/language/files/dependency-lock" %}

## tfvar files

Files used to assign variables:

* \*.auto.tfvars
* \*.auto.tfvars.json
* terraform.tfvars.json
* terraform.tfvars

For order of precedence see [Variables in HCL](hcl.md#order-of-precedence-for-variable-assignment).

