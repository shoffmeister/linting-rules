---
description: Security schema should have a description
given: $.components.securitySchemes[*]
severity: warn
then:
  field: description
  function: truthy
...
given: $.components.securitySchemes[*]
severity: warn
then:
  field: description
  function: truthy