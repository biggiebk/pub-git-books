# Expressions

{% embed url="https://developer.hashicorp.com/terraform/language/expressions" %}

## Conditional Expression

```
variable_name = condition ? true state : false state
```

Using the above the value for variable\_name would depend upon if the condition was true.  If true the result of the true state is assigned and false state is if the condition is false.
