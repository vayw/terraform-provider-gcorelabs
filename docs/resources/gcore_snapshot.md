---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "gcore_snapshot Resource - terraform-provider-gcorelabs"
subcategory: ""
description: |-
  
---

# gcore_snapshot (Resource)



## Example Usage

```terraform
provider gcore {
  user_name = "test"
  password = "test"
  gcore_platform = "https://api.gcdn.co"
  gcore_api = "https://api.cloud.gcorelabs.com"
}

resource "gcore_snapshot" "snapshot" {
  project_id = 1
  region_id = 1
  name = "snapshot example"
  volume_id = "28e9edcb-1593-41fe-971b-da729c6ec301"
  description = "snapshot example description"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **name** (String)
- **volume_id** (String)

### Optional

- **description** (String)
- **id** (String) The ID of this resource.
- **last_updated** (String)
- **project_id** (Number)
- **project_name** (String)
- **region_id** (Number)
- **region_name** (String)

### Read-Only

- **size** (Number)
- **status** (String)

