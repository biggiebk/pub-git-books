# Check

{% embed url="https://developer.hashicorp.com/terraform/language/checks" %}

Run a check after an apply.  Does not block any implementation only issues a warning error message.

```hcl
check "name_of_check" {
  data "type" "name" {
    url = "https://some.host.url/
  }

  assert {
    condition = data.type.name.status_code == 200
    error_message = "Site is not healthy"
  }
}
```

Data source is not mandatory and is used based on need.
