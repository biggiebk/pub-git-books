# Precondition and Postcondition

{% embed url="https://developer.hashicorp.com/terraform/language/expressions/custom-conditions#preconditions-and-postconditions" %}

These can be added under the lifecycle block on resources, modules, and data sources.

## Precondition

Checks to be run before rendering of the plan.

```hcl
lifecycle {
  precondition {
    condition     = data.aws_ami.example.architecture == "x86_64"
    error_message = "The selected AMI must be for the x86_64 architecture."
  }
}
```

## Postcondition

Checks to be run after rendering the plan, but before apply.

```hcl
lifecycle {
  postcondition {
    condition     = self.public_dns != ""
    error_message = "EC2 instance must be in a VPC that has public DNS hostnames enabled."
  }
}
```

The self keyword is only available in postcondition.
