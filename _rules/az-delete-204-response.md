---
description: A delete operation should have a 204 response.
message: A delete operation should have a `204` response.
severity: warn
formats:
- oas2
- oas3
given: $.paths[*].delete.responses
then:
  field: "204"
  function: truthy
...
message: A delete operation should have a `204` response.
severity: warn
formats:
- oas2
- oas3
given: $.paths[*].delete.responses
then:
  field: "204"
  function: truthy