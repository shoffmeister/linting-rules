---
paths-camel-case:
  description: Paths should be camel case
  message: '{{property}} is not camelCase {{error}}'
  severity: warn
  recommended: true
  format: oas2
  given: $.paths[*]~
  then:
    function: pattern
    functionOptions:
      match: ^(\/)?[A-Z][a-zA-Z0-9]*(\/)?
...
paths-camel-case:
  description: Paths should be camel case
  message: '{{property}} is not camelCase {{error}}'
  severity: warn
  recommended: true
  format: oas2
  given: $.paths[*]~
  then:
    function: pattern
    functionOptions:
      match: ^(\/)?[A-Z][a-zA-Z0-9]*(\/)?