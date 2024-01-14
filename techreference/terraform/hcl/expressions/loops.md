# Loops

## Count Meta Argument

{% embed url="https://developer.hashicorp.com/terraform/language/meta-arguments/count" %}

Loop through and create N resoruces using count.

```hcl
resource "type_of_resource" "name_of_resources" {
  count = 2 # create two resources of this type
  name = "my_name_is-${count.index}"

  tags = {
    Name = "Server ${count.index}"
  }
}
```

Would create two resources with the following names:

* type\_of\_resource.name\_of\_resource.my\_name\_is\[0]
* type\_of\_resource.name\_of\_resource.my\_name\_is\[1]

The count always starts at 0
