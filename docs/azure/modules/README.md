<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.6.0 |
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | ~> 4.2.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_azurerm"></a> [azurerm](#provider\_azurerm) | 4.2.0 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_ama"></a> [ama](#module\_ama) | ./Modules/ama | n/a |
| <a name="module_managed_virtual_machines"></a> [managed\_virtual\_machines](#module\_managed\_virtual\_machines) | ./Modules/Managed_Virtual_Machines | n/a |
| <a name="module_managed_vmss"></a> [managed\_vmss](#module\_managed\_vmss) | ./Modules/managed_virtual_machine_scalesets | n/a |

## Resources

| Name | Type |
|------|------|
| [azurerm_monitor_action_group.ag_monitoring](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/monitor_action_group) | resource |
| [azurerm_resource_group.rg_monitoring](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group) | resource |
| [azurerm_role_assignment.ra-pol-ama](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_subscription_policy_assignment.pol-ama](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/subscription_policy_assignment) | resource |
| [azurerm_user_assigned_identity.id-ama](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/user_assigned_identity) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_action_group_name"></a> [action\_group\_name](#input\_action\_group\_name) | Name of the action group | `string` | `"Atea-DefaultActionGroup"` | no |
| <a name="input_action_group_short_name"></a> [action\_group\_short\_name](#input\_action\_group\_short\_name) | Short name of the action group | `string` | `"Atea-Default"` | no |
| <a name="input_amaconfig"></a> [amaconfig](#input\_amaconfig) | n/a | <pre>object({<br/>    dcr = object({<br/>      name = optional(string, "dcr-vmmon-001")<br/>      destinations = object({<br/>        azure_monitor_metrics = object({<br/>          name = optional(string, "Microsoft-InsightsMetrics")<br/>        })<br/>      })<br/>      data_flows = object({<br/>        performance_counter = object({<br/>          streams       = optional(list(string), ["Microsoft-InsightsMetrics"])<br/>          destinations  = optional(list(string), ["Microsoft-InsightsMetrics"])<br/>          transform_kql = optional(string, "source")<br/>          output_stream = optional(string, "Microsoft-InsightsMetrics")<br/>        })<br/>        syslog = object({<br/>          streams       = optional(list(string), ["Microsoft-Syslog"])<br/>          transform_kql = optional(string, "source")<br/>          output_stream = optional(string, "Microsoft-Syslog")<br/>        })<br/>        windows_event_log = object({<br/>          streams       = optional(list(string), ["Microsoft-Event"])<br/>          transform_kql = optional(string, "source")<br/>          output_stream = optional(string, "Microsoft-Event")<br/>        })<br/>      })<br/>      data_sources = object({<br/>        performance_counter = object({<br/>          counter_specifiers = optional(list(string), [<br/>            "Processor(*)\\% Processor Time",<br/>            "Processor(*)\\% Idle Time",<br/>            "Processor(*)\\% User Time",<br/>            "Processor(*)\\% Nice Time",<br/>            "Processor(*)\\% Privileged Time",<br/>            "Processor(*)\\% IO Wait Time",<br/>            "Processor(*)\\% Interrupt Time",<br/>            "Memory(*)\\Available MBytes Memory",<br/>            "Memory(*)\\% Available Memory",<br/>            "Memory(*)\\Used Memory MBytes",<br/>            "Memory(*)\\% Used Memory",<br/>            "Memory(*)\\Pages/sec",<br/>            "Memory(*)\\Page Reads/sec",<br/>            "Memory(*)\\Page Writes/sec",<br/>            "Memory(*)\\Available MBytes Swap",<br/>            "Memory(*)\\% Available Swap Space",<br/>            "Memory(*)\\Used MBytes Swap Space",<br/>            "Memory(*)\\% Used Swap Space",<br/>            "Process(*)\\Pct User Time",<br/>            "Process(*)\\Pct Privileged Time",<br/>            "Process(*)\\Used Memory",<br/>            "Process(*)\\Virtual Shared Memory",<br/>            "Logical Disk(*)\\% Free Inodes",<br/>            "Logical Disk(*)\\% Used Inodes",<br/>            "Logical Disk(*)\\Free Megabytes",<br/>            "Logical Disk(*)\\% Free Space",<br/>            "Logical Disk(*)\\% Used Space",<br/>            "Logical Disk(*)\\Logical Disk Bytes/sec",<br/>            "Logical Disk(*)\\Disk Read Bytes/sec",<br/>            "Logical Disk(*)\\Disk Write Bytes/sec",<br/>            "Logical Disk(*)\\Disk Transfers/sec",<br/>            "Logical Disk(*)\\Disk Reads/sec",<br/>            "Logical Disk(*)\\Disk Writes/sec",<br/>            "Network(*)\\Total Bytes Transmitted",<br/>            "Network(*)\\Total Bytes Received",<br/>            "Network(*)\\Total Bytes",<br/>            "Network(*)\\Total Packets Transmitted",<br/>            "Network(*)\\Total Packets Received",<br/>            "Network(*)\\Total Rx Errors",<br/>            "Network(*)\\Total Tx Errors",<br/>            "Network(*)\\Total Collisions",<br/>            "System(*)\\Uptime",<br/>            "System(*)\\Load1",<br/>            "System(*)\\Load5",<br/>            "System(*)\\Load15",<br/>            "System(*)\\Users",<br/>            "System(*)\\Unique Users",<br/>            "System(*)\\CPUs"<br/>          ])<br/>          name                          = optional(string, "perfCounterDataSource60")<br/>          sampling_frequency_in_seconds = optional(number, 60)<br/>          streams                       = optional(list(string), ["Microsoft-InsightsMetrics"])<br/>        })<br/>        syslog = object({<br/>          facility_names = optional(list(string), [<br/>            "alert",<br/>            "audit",<br/>            "auth",<br/>            "authpriv",<br/>            "clock",<br/>            "cron",<br/>            "daemon",<br/>            "ftp",<br/>            "kern",<br/>            "local0",<br/>            "local1",<br/>            "local2",<br/>            "local3",<br/>            "local4",<br/>            "local5",<br/>            "local6",<br/>            "local7",<br/>            "lpr",<br/>            "mail",<br/>            "news",<br/>            "nopri",<br/>            "ntp",<br/>            "syslog",<br/>            "user",<br/>            "uucp"<br/>          ])<br/>          log_levels = optional(list(string), [<br/>            "Error",<br/>            "Critical",<br/>            "Alert",<br/>            "Emergency"<br/>          ])<br/>          name    = optional(string, "sysLogsDataSource")<br/>          streams = optional(list(string), ["Microsoft-Syslog"])<br/>        })<br/>        windows_event_log = object({<br/>          streams = optional(list(string), ["Microsoft-Event"])<br/>          name    = optional(string, "eventLogsDataSource")<br/>          x_path_queries = optional(list(string), [<br/>            "Application!*[System[(Level=1 or Level=2 or Level=3) and (EventID != 6006)]]",<br/>            "System!*[System[(Level=1 or Level=2 or Level=3)]]"<br/>          ])<br/>        })<br/>      })<br/>    })<br/>    law = object({<br/>      name = optional(string, "law-vmmon-001")<br/>    })<br/>  })</pre> | n/a | yes |
| <a name="input_location"></a> [location](#input\_location) | Region for the alert rules. Default West Europe (Amsterdam) | `string` | `"westeurope"` | no |
| <a name="input_resource_group_tags"></a> [resource\_group\_tags](#input\_resource\_group\_tags) | Tags for the resource group. | `map(any)` | <pre>{<br/>  "costcenter": "tbd",<br/>  "owner": "tbd"<br/>}</pre> | no |
| <a name="input_subscription_id"></a> [subscription\_id](#input\_subscription\_id) | The Subscription ID of the resouces | `string` | n/a | yes |
| <a name="input_target_resource_group_name"></a> [target\_resource\_group\_name](#input\_target\_resource\_group\_name) | The resouce group where you want to store the alerts | `string` | n/a | yes |
| <a name="input_target_resource_id_list"></a> [target\_resource\_id\_list](#input\_target\_resource\_id\_list) | n/a | `list(any)` | `[]` | no |
| <a name="input_tenant_id"></a> [tenant\_id](#input\_tenant\_id) | Tenant ID for the target directory | `string` | n/a | yes |
| <a name="input_webhook_name"></a> [webhook\_name](#input\_webhook\_name) | The webhook name for alerts during testing | `string` | n/a | yes |
| <a name="input_webhook_url"></a> [webhook\_url](#input\_webhook\_url) | The webhook for alerts during testing | `string` | n/a | yes |

## Outputs

No outputs.
<!-- END_TF_DOCS -->

## Example tfvars file
```hcl

webhook_url                = "https://ams-webhooks.myatea.net/a-hook/azure"
webhook_name               = "AMS Zabbix"
subscription_id            = "56e3100b-a986-4f9b-b7dd-ca013a5e4450"
tenant_id                  = "65f51067-7d65-4aa9-b996-4cc43a0d7111"
target_resource_group_name = "rg-ritual-mon-location-01"
location                   = "some-location"

target_resource_id_list = [
  "/subscriptions/66666666-6666-6666-6666-666666666666/resourceGroups/rg-ritual-sql-location-01/providers/Microsoft.Compute/virtualMachines/vm-ritual-sql-location-01"
]

amaconfig = {
  dcr = {
    data_flows = {
      performance_counter = {}
      syslog = {}
      windows_event_log = {}
    }
    data_sources = {
      performance_counter = {}
      syslog = {}
      windows_event_log = {}
    }
    destinations = {
      azure_monitor_metrics = {}
    }
  }
  dce = {}
  law = {}
}

```