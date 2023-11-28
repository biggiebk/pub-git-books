---
description: List of terraform commands with some common options
---

# CLI

{% embed url="https://developer.hashicorp.com/terraform/cli" %}

## init

{% embed url="https://developer.hashicorp.com/terraform/cli/commands/init" %}

Retrieves child modules and plugins (providers).

### -upgrade

Upgrades all previously installed modules and plugins (providers) based on the specified version constraints.

## plan

{% embed url="https://developer.hashicorp.com/terraform/cli/commands/plan" %}

Creates an execution plan to preview changes.

### -destroy

Creates a plan for destroying, similar to the destroy command, but read only.

### -out

Saves the plan to a file to pass to apply later

### -var

Specify a value for a input variable
