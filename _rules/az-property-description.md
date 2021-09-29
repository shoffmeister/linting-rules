---
description: All schema properties should have a description.
message: Property should have a description.
severity: warn
resolved: false
given: $..[?(@.type === 'object' && @.properties)].properties[*]
then:
  field: description
  function: truthy
...
message: Property should have a description.
severity: warn
resolved: false
given: $..[?(@.type === 'object' && @.properties)].properties[*]
then:
  field: description
  function: truthy