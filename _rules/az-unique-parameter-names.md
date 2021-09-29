---
description: All parameter names for an operation should be case-insensitive unique.
message: '{{error}}'
severity: warn
formats:
- oas2
given: $.paths[*]
then:
  function: unique-param-names
...
message: '{{error}}'
severity: warn
formats:
- oas2
given: $.paths[*]
then:
  function: unique-param-names