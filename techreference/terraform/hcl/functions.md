# Functions

{% embed url="https://developer.hashicorp.com/terraform/language/functions" %}

## Merge Maps

```
> merge({a="b", c="d"}, {e="f", c="z"})
{
  "a" = "b"
  "c" = "z"
  "e" = "f"
}

> merge({a="b"}, {a=[1,2], c="z"}, {d=3})
{
  "a" = [
    1,
    2,
  ]
  "c" = "z"
  "d" = 3
}

```
