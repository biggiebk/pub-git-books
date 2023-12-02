---
description: Some basic structures for Hashicorp Configuration Language (HCL)
---

# HCL

{% embed url="https://developer.hashicorp.com/terraform/language" %}

## Provider

{% embed url="https://developer.hashicorp.com/terraform/language/providers" %}

```
provider "<provider_name>" {
  alias = "..."
  ...
}
```

### Alias

Allows for multiple versions of a provider  to be used by assigning an alias name.&#x20;

{% embed url="https://developer.hashicorp.com/terraform/language/providers/configuration#alias-multiple-provider-configurations" %}

## Resource

{% embed url="https://developer.hashicorp.com/terraform/language/resources/syntax" %}

```
resource "type_of_resrouce" "name_of_resrouce" {
    ...
}
```

The available arguments depends on the resource. See the [Hashicorp Registry](https://developer.hashicorp.com/terraform/language) for more information on the resource.

### Meta Arguments

Here are a list of meta arguments that all resources support.

* [depends\_on ](https://developer.hashicorp.com/terraform/language/meta-arguments/depends\_on)- Specifies a dependency that Terraform is not properly handling.
* [count ](https://developer.hashicorp.com/terraform/language/meta-arguments/count)-  Create resources based on a number
* [for\_each ](https://developer.hashicorp.com/terraform/language/meta-arguments/for\_each)- Loop through a map or a set of strings to create multiple resources
* [provider ](https://developer.hashicorp.com/terraform/language/meta-arguments/resource-provider)- Selects which provider to select the resource from to override Terraforms default behavior.
* [lifecycle](https://developer.hashicorp.com/terraform/language/meta-arguments/lifecycle) - Helps with lifecycle of the resource
* [provisioner](https://developer.hashicorp.com/terraform/language/resources/provisioners/syntax) - Allows for  extra actions after creation of the resource

## Terraform

{% embed url="https://developer.hashicorp.com/terraform/language/settings" %}

```
terraform {
  required_version = "<version>"
  
  required_providers {
    <provider_name> = {
      version = "<version>"
    }
  }
}
```

## Variable

{% embed url="https://developer.hashicorp.com/terraform/language/values/variables" %}

```
variable "name_of_variable" {
    default - Default value if no value provided
    type - Specifies the type of data
    description - The documentation for the variable
    validation - Defines a block of validation rules
    sensitive - Prevents outputting of value to protect sensitive data
    nullable - Determines if the variable can be null or not
}
```

### Order of Precedence for Variable Assignment

1. \-var or var-file
2. \*.auto.tfvars or \*.auto.tfvars.json
3. terraform.tfvars.json
4. terraform.tfvars
5. Environment Variables

### Types

The following are the possible variable types.&#x20;

* string
* number
* bool
* list(\<TYPE>)
* set(\<TYPE)
* map(\<TYPE>)
* object({\<ATTR\_NAME> = \<TYPE>, ... })
* tuple(\[\<TYPE>, ...])

{% embed url="https://developer.hashicorp.com/terraform/language/expressions/type-constraints" %}

### Variable Validation

{% embed url="https://developer.hashicorp.com/terraform/language/expressions/custom-conditions#input-variable-validation" %}
